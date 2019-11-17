## notes on _the inmates are running the asylum_

The book's author is the developer of goal-directed design. The discussion of goal-oriented design is saved until part iv-v of the book. The author spends most the time convincing the reader that tech products suck (part i); convincing the reader that if you're making tech products, making crappy products puts you at a disadvantage (part ii); and getting inside the head of a programmer (part iii). 

Main ideas:

- Most software is bad.
- To make software less bad, it should be designed with the users goals in mind.
- Get rid of thinking about 'features'; think about users and what goals they want to achieve with your product.
- Spend a lot of time planning and designing the product _before_ the programmers hit the keyboards.

### chapter 1

- Lots of examples of poor design in for more 'techy' products. I'd note that there are plenty of poorly-designed products, although for reasons that become clear later in the book, tech products might be particular flagrant offenders.
- "We are deficient in our development _process_, not in our development tools."
- The cause of a lot of the poor design for tech products is that the goals of the programmer and the goals of the user are different. Most tech products are de facto designed by software engineers. This is bad.
- Need to do 'interaction design' _before_ the programmers get to work

### chapter 2

- _cognitive friction_ - resistance encountered when a human engages with a "complex system of rules that change as a problem changes". A microwave as lot of a cognitive friction: the button meaning often depend on what 'mode' you're in. A violin is complex and difficult to control, but at least it's _predictable_ unlike the microwave.
- Interface design is slapping a groovy-looking UI on something. It's not the same as interaction design, which describes how a user interacts with the product. A product can look amazing and still be terribly designed.
- Interface designers think (a) conceptually, (b) then in terms of behavior, (c) _then_ interface
- _dancing bear_: With most tech software, we're just amazed that it works--look! the bear is dancing! We typically don't think, "That bear sucks at dancing;" the fact that it's dancing at all is what's amazing.
- Cooper makes the case that most people that doesn't regularly swear at our computers are apologists. We accept the dancing bear because we are impressed that the bear can dance. When other people point out the dancing sucks, we make excuses for the bear. Cooper has great empathy for the 'naive users' who are constantly frustrated by computer software.

### chapter 3

- For software-based products, we have to blend two types of product specs: (a) how the user will react / feel about the product and (b) a detailed and complete description of that the product will look like. Cooper argues that software is rarely truly designed; the culture of shipping software is around around 'features', and what usually passes for design is determining the list of features that will go into the final product. This is not true design!
- "...users don't care that much about features. Users only care about achieving their goals.". Features can sometimes help a user achieve their goal, but often they are just confusing.
- More features != successful product
- Cooper finds the view expressed by some--we'll ship something, see how users respond, and iterate from there--to be repulsive. Cooper thinks this is like asking your users to wade through a bunch of pain to help you design your product.
- Microsoft spends $800 M / year on technical support (this book was written in 2004)
- "It is more costly in the long run to have programmers write the wrong thing than to write nothing at all. This truth is so counter-intuitive that most managers balk at the very idea."
- Cooper doesn't like prototypes in practice because prototypes--which are not truly designed--are often put into production by senior management that doesn't understand the purpose / limitations of the prototype. They _should_ be viewed as experiments. "The value of the prototype is in the education it gives you, not in the code itself."


### chapter 4

Basically a bunch of examples of bad design in tech products. Email clients that don't support threaded messages (virtually all clients do this now), calendar software that doesn't tell you when to leave or specify a vague or undetermined end time for an event, browsers that don't proactively load pages or test for broken links.

Cooper argues that software:

- forgets: it doesn't remember your past behavior
- is lazy
- is parsimonious with information 
- is inflexible
- blames users
- doesn't take responsibility (e.g. "are you sure you want to delete this file?")
- makes people feel stupid

### chapter 5

- Keely's model for high-tech products: what's capable (engineering), what's viable (business), and what's desirable (design). Cooper argues that the right way to approach a product is to start with what customers will find desirable, _then_ decide whether you can build and sell it. (This has a lot in common with Rob's 'market validation' approach.)
- Desirability != need. Over the long-term, desires trump needs
- Dancing bearware will never generate customer loyalty
- "Design makes your products desirable, and that will make your customer actively seek out your products instead of the competitor's, regardless of who got there first." Example: Apple, which rarely (truly) innovates. Also connection to the illusion of first-mover advantage.

### chapter 6

- Products are rarely designed _a priori_ as they should be. The design doc is typically written _post-hoc_
- Most management focuses on timelines and numbers of features added. These are easy to track but unrelated to the product actually delivering something of value to the customer.
- Software engineers are ultimately the ones running the show. They will often focus on things that amuse them instead of focusing on things that actually matter for the success of the product.

### chapter 7

This chapter is all about getting in the head of a programmer.

- "Programmers trade simplicity for control. They exchange success for understanding."
- "the jetway test": would you rather learn to fly the plane or let someone else fly the plane and relax? Programmers will take the former route.
- Normal humans are content to not know how something works. Programmers don't understand this perspective, and they build software accordingly.
- Programmers are often obsessed what _what could possibly happen_ instead of _what's likely to happen_, i.e., they spend an inordinate amount of time probing edge cases that might not actually matter


### chapter 8

- Reusing code makes a lot of sense and programmers often do it, but at the expense of the user experience of the final product
- Programmers have a high reverence for technical skill
- Programmers often don't have respect for less technical people
- Programmers often look at suggestions from less technical people more as suggestions than directives. "Instead of seeing the written design specification as a blueprint, he sees it as the op-ed page of a newspaper."

### chapter 9

This is where we're introduced to _goal-directed design_

- _personas_: a precise description of a user and what they want to accomplish. Personas form the core of goal-directed design. They are archetypes of a users that _are defined by goals_. (Ironically, these personas are trading simplicity for complexity.)
- _design for just one person_. This stuck me as really stupid at first, but I came around to the idea eventually. Designing for everyone will lead to a crappy design. Different users have different goals.
- Interesting anecdote: 80% of people in focus groups hated the Dodge Ram, but the other 20% loved it, so Dodge went ahead with it.
- "Having people love your product, even if it only a minority, is how you succeed."
- Loyal customers are the most powerful marketing tool known
- The persons should be really specific: everyone should be able to form a concrete mental image of the persona. If the persona isn't concrete, different teams can flesh out a persona in different ways.
- In designing personas, Cooper argues that precision is more important than accuracy
- Using personas ends debates about what features to include in the product
- Personas are useful for both programmers _and_ designers
- Personas should be _users_ not _buyers_
- Each product will have, at most, three primary personas that we design for. Initially, you might create a ton of personas, but you merge them as you realize their goals are similar. If you have more than three at the end, you're problem is too big.
- Example of the in-flight entertainment system Cooper designed


### chapter 10

- Goals are the reasons a user performs tasks
- Tasks != goals. We complete tasks in order to eventually achieve some goal. Tasks and goals can often be in opposition (e.g. the president might deploy troops oversees but his goal is peace). Only goals are steady, not tasks.
- Different types of goals:
  - personal goals, e.g., not feel stupid, have fun, not make mistakes
  - corporate goals, e.g., increase profit, hire more people
  - practical goals, e.g., avoid meetings, handle client demands
  - false goals, e.g., save (computer) memory, save keystrokes, be easy to learn, increase UI beauty
- Cooper argues that we fail if we don't make sure we design for the user's _personal_ goals
- Cooper argues software should be 'polite'. He spends a lot of time talking about what this means. Software that is: interested in me, forthcoming, gives instant gratification, has common sense, anticipates my needs, responsive, well-informed, confident, trustworthy, etc.
- 'Drumbeat' example

### chapter 11

- _Scenarios_ are precise descriptions of a persona using a product to achieve a goal. Three types:
  - daily use: most important
  - necessary use: less important, but still important (things that must be done, but are done infrequently)
  - edge case: the _product_ won't fail or success based on handling edge-case scenarios. Pay no mind.
- _inflecting the interface_- easy to use without sacrificing functionality
- Programmers design for experts, marketers design for beginners: the most important group is the 'perpetual intermediates' who are in between these extremes
- Often useful when brainstorming to "pretend the computer is magic" and can do whatever we want it to do. Helps focus things and ensures wee don't get distracted by thee tech and instead focus on the user.
- Example of the tiny scanner


### chapter 12

The idea of this chapter is that design has to come before programming, testing, and tweaking.

### chapter 13

- Big difference between listening to your customers and doing what your customers tell you to do. The latter will get you into problem. Recall the Ford quotation about customers wanting a faster horse. 
- Customer-driven products don't have a coherent design
- Customer-driven design isn't really design. 
- Comparison to making movies: Most of the work is in planning (pre-production) since filming is so expensive. Software should be the same way since programmers are expensive. 
- Author a design document. Should be detailed. Will affect how the code is written. Will benefit programmers, marketing, documenters, tech support.


---------

## interesting quotations

- "...users don't care that much about features. Users only care about achieving their goals."
- "It is more costly in the long run to have programmers write the wrong thing than to write nothing at all. This truth is so counter-intuitive that most managers balk at the very idea."
- "It is common mistake to copy the trappings of success, rather than the root cause of it."
- "Trying to please too many points of view can kill an otherwise good product."
- "Having people love your product, even if it only a minority, is how you succeed." 
- "From an interaction designer's point of view, the divisions between hardware and software are inconsequential because they are inconsequential to the user."
- "...the complexity of a program increases exponentially relative to its size in lines of code."
- "Iteration never creates great products." Though he backtrack on this a bit: "Getting to the right product is always a matter of iterating. It always takes several tries to get the details right."
- "You can always postpone short-term thinking, but you can never postpone long-term thinking."
