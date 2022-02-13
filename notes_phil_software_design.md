# a philosophy of software design

Ousterhout

I liked this book overall, and while I didn't agree with everything, I thought it made it a lot of good points and some unique but well-considered opinions I hadn't encountered before. The focus on _complexity of systems_ makes a lot of sense, but I think knowledge of the "Law of Conservation of Complexity" would have been helpful in a lot of discussions and arguments.

- [a philosophy of software design](#a-philosophy-of-software-design)
    - [chapter 1](#chapter-1)
    - [chapter 2: the nature of complexity](#chapter-2-the-nature-of-complexity)
    - [chapter 3: working code isn't enough](#chapter-3-working-code-isnt-enough)
    - [chapter 4: modules should be deep](#chapter-4-modules-should-be-deep)
    - [chapter 5: information hiding](#chapter-5-information-hiding)
    - [chapter 6: general-purpose modules are deep](#chapter-6-general-purpose-modules-are-deep)
    - [chapter 7: different layer, different abstraction](#chapter-7-different-layer-different-abstraction)
    - [chapter 8: pull complexity downwards](#chapter-8-pull-complexity-downwards)
    - [chapter 9: better together or apart](#chapter-9-better-together-or-apart)
    - [chapter 10: define errors out of existence](#chapter-10-define-errors-out-of-existence)
    - [chapter 11: design it twice](#chapter-11-design-it-twice)
    - [chapter 12: why write comments](#chapter-12-why-write-comments)
    - [chapter 13: comments should describe things that aren't obvious from the code](#chapter-13-comments-should-describe-things-that-arent-obvious-from-the-code)
    - [chapter 14: choosing names](#chapter-14-choosing-names)
    - [chapter 17: consistency](#chapter-17-consistency)
    - [chapter 18: code should be obvious](#chapter-18-code-should-be-obvious)
  - [list of red flags](#list-of-red-flags)


### chapter 1

- he argues that out greater limitation in writing code is an inability to understand the systems we're implementing
- complexity makes it more difficult for programmers to keep all the relevant information in mind as they change the system
- he's basically arguing that software represents systems than need to be able to evolve and be modified over time


### chapter 2: the nature of complexity

- __complexity is anything related to the structure of a software system that makes it hard to understand and modify the system__
- if code is complex to other people, it's complex, even it's simple to you
- isolating complexity where it's never seen is almost as good as eliminating it altogether
- systems of complexity:
  - change amplification (a simple change requires changes in several places)
  - cognitive load
  - unknown unknowns - not clear what you need to know to change a piece of code. in an obvious system, a developer can make a quick and accurate guess about where they need to make a change to the codebase
- causes of complexity: __dependencies__ and __obscurity__ (important information is not obvious)


### chapter 3: working code isn't enough

- strategic vs tactical (just make it run) programming
- "Strategic programming requires an investment mindset. Rather than taking the fastest path to finish your current project, you must invest time to improve the design of the system. He's investments will slow down a bit in the short term, but they will speed you up in the long term."
- the best engineers care deeply about good design


### chapter 4: modules should be deep

- modules have two components
  - **interface** - the args, return type what you need to know to call that method/function (the _what_, not the _how_). Think: everything that's in a Python docstring (including stuff like exceptions or notes)
  - **implementation** - the code that carries out what's promised by the interface
- he argues that modules should be _deep_: their interfaces should be much simpler than their implementations. In this way, you hide complexity from the rest of the system, and can make changes to the implementation without having to refactor (as long as the interface stays the same)
- think of many unix tools, or garbage collection: there's a ton happening behind the scenes, but the interface for is actually quite shallow and easy to use / think about
- **An abstraction is a simplified view of an entity, which omits an important important details**
- w/r/t to args, he sort of wants it both ways: he says choice is good, but **interfaces should be designed to make the most common case as simple as possible.** 

### chapter 5: information hiding

- information leakage: when a design decision is reflected in multiple modules
- this chapter went a bit over my head unfortunately

### chapter 6: general-purpose modules are deep

- **classes should be 'somewhat general purpose': he means that the module functionality should reflect your current needs, but the interface should be general enough to support multiple / future use cases**
- **One of the most important elements of software design is determining who needs to know what, and when. When the details are important, it is better to make them explicit and as obvious as possible.**
- questions to ask
  - what is the simplest interface to cover al my current needs
  - in how many situations will this method be used
  - this api easy to use for my current needs?

### chapter 7: different layer, different abstraction

- In a well-designed system, each layer provides a different abstraction from the layers above and below it
- pass through methods are an anti-pattern
- pass-through variables are also bad, because they force all intermediate methods to be aware of their existence, even if the methods have no use for the variables
- global variables almost always create other problems


### chapter 8: pull complexity downwards

- it's much more important for a module to have a simple interface than a simple implementation. it's easy as a developer to do the opposite: expose all the complexity to the user / caller and let them figure it out, but this leads to complex code and shallow modules
- the point of this chapter is you really have to understand what your users are trying to do with your code and then do it automatically without exposing a lot of implementation details to them


### chapter 9: better together or apart

- bring things together if it simplifies the interface
- separate general-purpose and special-purpose code
- splitting up code introduces additional interfaces, which will increase complexity of the system
- he argues that long functions / methods aren't bad if they are easy to head and have simple interfaces. the alternative is often breaking things up into little pieces, which require someone to understand a bunch more interfaces and flip back and forth between different methods
- **each method should do one thing and do it completely**
- splitting up a method
  - extract a subtask from the main method (can work)
  - divide into two methods (rarely works)
  - create several shallow methods (avoid; the complexity 'hidden' in the implementation spills out into the interfaces)

### chapter 10: define errors out of existence

- exception handling is more difficult to write than normal code
- two outcomes:
  - handle the exception, keep doing work
  - halt the program and allow the caller to deal with it
- he's basically arguing that it's lazy and unhelpful to report exceptions back to the caller, because you force the caller to deal with the exception, instead of understanding what the program should do instead
- classes with lots of exceptions have complex interfaces and are shallow as a result

### chapter 11: design it twice

- pick two radically different approaches and do some basic experimentation: neither might be the final design, but you'll learn more that way
- designing the system is high-leverage and taking a little extra time likely pays dividends

### chapter 12: why write comments

- common excuses for not writing comments:
  - good code is self-documenting. but there's still a sig. amount of design info that the code itself is unable to represent. If users must read the code of a method in order to use it, then there is no abstraction.
  - don't have time.
  - comments get out of date
  - comments are generally worthless
- the value of comments is in being able to capture information that was in the mind of the designer but couldn't be represented in the code
- good comments helps with unknown unknowns and cognitive load in code

### chapter 13: comments should describe things that aren't obvious from the code

- use conventions
- do not just repeat what the code is doing
- use different words in the comment from those in the name of the entity being described
- comments should occur at a different level of detail from the code
- when documenting a variable, think _noun_ not _verb_; when documenting a function or method, think _verb_ bot _noun_
- if you want code that presents good abstractions, you must document those of extractions with comments
- interface comments provide information that someone needs to know in order to use a class or method; they define the abstraction (think: python docstrings)
- side effects must be documented in the interface comment
- it can be helpful to have examples in the class documentation that illustrate how its methods work together, particularly for deep classes with usage patterns that are non-obvious. think: example `demo()` `@classmethod` in python
- interface comments describe _what_ the code is doing, not _how_ it does it
- if you fix a bug that results in something non-obvious in the code, add a comment and a link to the bug report

### chapter 14: choosing names

- good names are of a form of documentation
- good names are precise, unambiguous, and intuitive -- they can be hard to get right as a result!
- think: "if someone sees this name in isolation, without seeing his declaration, it's documentation, or any code that uses the name, how closely will they be able to guess what the name refers to? Is there some other name that will paint a clear picture?"
- if the life of a variable is very short, tiny variable names like `i` and `j` are ok


### chapter 17: consistency

- Consistency is a powerful tool for reducing the complexity of the system and making his behavior more obvious. If the system is consistent, it means that some where things are done similar ways, and dissimilar things are done in different
- follow conventions in a codebase, and don't invent your own conventions that you think are better

### chapter 18: code should be obvious

- If code is obvious, it means that someone can read the code quickly, without much thought, and their first guess is about the behavior or meaning of the code will be correct
- things that make code more obvious:
  - whitespace
  - comments
- things that make code less obvious:
  - generic containers (e.g., using `tuple` instead of `NamedTuple`). **software should be designed for ease of reading, not ease of writing**
  - code that violates expectations
  - different types for declaration and allocation 



## list of red flags

- shallow modules: complex interface relative to the functionality it provides
- information leakage: when the same knowledge is used in multiple places, such as two different classes that both understand the format of a particular file
- temporal decomposition: execution order is reflected in the code structure: Operations that happen at different times are in different methods or classes. If the same knowledge is used a different points in execution, it gets encoded and multiple places, resulting an information leakage
- overexposure: If the API for commonly used features forces users to learn about other features that are rarely used, this increases the cognitive load on users who don't need the rarely used features.
- pass-through methods: do nothing except pass their arguments to a different method. indicates there's not a clean division of responsibility between modules
- repetition: if the same piece of code appears over and over again, you haven't found the right abstractions
- conjoined methods: when you can't understand one method without also understanding a different method
- comments repeat the code
- implementation documentation contaminates interface: i.e., when an interface comment describes the _how_
- vague names: if a method or variable name is broad enough that it could refer to many different things, it doesn't convey much information and is likely to be misused
- hard to pick name: if it's hard to name the thing, you might not have found a clean design
- hard to describe: if it's hard to describe a method or class, maybe you haven't found the right abstraction
- nonobvious code: if code can't be understand after a quick reading, that means there's important information that is not immediately clear to someone reading the code