# Software engineering at Google


### testing overview

- you test to catch bugs, but also to support change in your software--it's impossible to have confidence in a refactor without tests in place
- writing tests also improves the design of your systems, because poor code is often hard to test
- other benefits:
  - less debugging
  - increased confidence in changes
  - improved documentation
  - simpler reviews
  - thoughtful design 
  - faster, higher quality releases
- dimensions of a test
  - size of the test: small, medium, or large. resources required to run the test. small = single-threaded. no bound on large.
  - scope of the test: small, medium, or large. refers to the number of code paths we're _verifying_ (not necessary executing). e.g., if your function calls a bunch of helper functions, you still might be verifying a small piece of the code even though all that helper functions get executed. ideally, want 80% of tests to be small (aka unit) tests, 15% integration, 5% end-to-end 
- flaky tests are very bad and problematic, even if their rate in the codebase is relatively low. at google, flakey test rate is ~0.15%
- anti-pattern: control flow in tests. makes it more likely that there's an error in your tests. keep tests as simple as possible.
- beyonce rule - if you liked it, you should have put a test on it. test any behavior you care about


### unit testing

- avoid brittle tests -- if tests break in response to bug fixes, new features, or refactors, something's wrong. test _should_ break when the behavior of the code changes in some way
- test via the public APIs--do not test the implementation details. you should be able to totally change how the function is implemented and still have your tests pass as long as the function interface remains the same
- _interaction tests_ (making sure the code took an expected set of actions with other code) tends to produce more brittle tests; also rely on mocks
- _state testing_ is about testing the outwardly observable state or behavior of the system
- a tests's clarity (the speed required to identify what's causing a test failure) depends on
  - test completeness - everything needed to understand the test is contained in the body of the test
  - test conciseness - only the relevant information is in the test, and nothing else
- test _behaviors_, not methods. if a method has multiple behaviors, you should be writing a test for each one, as opposed to creating a single test associated with the method
- use given/when/then to focus on testing behaviors
- most tests should have a single _when_ and a single _then_ block
- name your tests based on the behavior they are testing -- try starting the test name with 'should'
- don't put logic in tests
- it's less important for test code to be DRY -- it should be DAMP (descriptive and meaningful phrases)
  - there's a lot you can do to create test data or setup outside the test. this make your code DRYer, but the completeness of your tests tanks
  - it's okay to be a little less DRY in your tests as long as it improves the clarity of your tests
  - helper methods are okay, but they shouldn't use mock data that a reader would have to look elsewhere in the code to understand 


### test doubles

- a test double is an object or function that can stand in for a real implementation in a test (like a stunt double in a movie)
- there are a bunch of ways to use test doubles; some are more appropriate than others
- a _seam_ is a way to make code more testable by allowing the code to make use of test doubles
- _dependency injection_ is a way to introduce a seam -- e.g., a class's dependencies are passed to it during initatiion rather than instantiated directly
- mocks are test doubles whose behavior is specified inline in a test
- techniques
  - faking
    - using a simplified, fake version of the actual object or implementation under test
  - stubbing
    - giving behavior to a function that otherwise has no behavior on it's own -- you generally _stub_ the return value to replicate behavior you'd expect to see from some actual object
  - interaction testing
    - validating _how_ a function is called without actually calling the implementation of the function (e.g., verifying that a dependency of a method was called with certain parameters, or a certain number of times) 
- they prefer using real implementations where possible, because it most closely mimics what you'll find in prod
  - but sometimes you can't use real implementations
  - they can make your tests slow
  - they can make some tests flaky if you're interacting with external systems
- if you can't use the real thing, you can use a _fake_
  - a fake is as close to the real object as possible, but won't interact with services or call your transaction auth service, e.g., and is fast
  - fakes have to be maintained as the code changes -- generally the code owners need to maintain both the code and the fake
  - fakes also need to have their own tests to make sure they conform to the API of the real mccoy
- stubbing is generally overused
  - tests become unclear, brittle, less effective; in short, require more work in the long-term to deal with
  - stubbing can be used when you need a function to return a value to get the system under test into a certain state -- stubbing makes it easy to verify behavior under a wide array of return values
- interaction testing
  - always prefer _state testing_--testing the outwardly observable behavior of code--to _interaction testing_, which verifies how a function is called without actually calling the implementation of the function
  - interaction testing can't actually tell you if things are working as expected -- it can only validate that certain functions are called as expected. at the end of the day, what you care about if the outwardly observable behavior
  - it also uses the implementation details of the test, an anti-pattern which means that any refactor will require updates / changes to the tests
  - it can be appropriate if differences in the number of or order of calls to a function would cause undesired, or to test something like a cacheing function to make sure it's working correctly
  - only perform interaction testing for functions that are _state-changing_