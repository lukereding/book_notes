# technology strategy patterns

roles of a software architect:
- constrain entropy
- determine non functional requirements. things you can’t tell a PO to build. scaleability, maintainability, interpretability, etc. 
- determine trade offs

"you’re never quite solving a problem. You’re only trading it for when you’d rather have."

"strategy is the art of creating power.” -lawrence freedman

strategy is about determining the problems and opportunities in front of you, the finding them properly, and shaping a course of action that will give your business the greatest advantage.

you really need strategy, culture, and execution.


## part ii: creating the strategy


using 'the five questions' framework:

- define the problem
- define your terms
- list the possible outcomes
- if there’s uncertainty, assign rough liklihihoods to each outcome. using inductive (specific -> general) and deductive reasoning to support why you think what you think
- prioritize based on (1) ease of execution and (2) size of impact. put the options on a scatter point with these axes


### chapter 3: world context

#### PESTEL

The idea here is to take a really broad survey of the world through the lens of your business. These categories help ensure you cover your bases:

- political
- economic
- social
- technology
- environmental
- legal

the steps are 

- gather a bunch of data. these might come from industry reports, conferences, papers, etc.
- develop and state your insights
- make local recommendations based on your insights


#### scenario planning

the idea here is to ask a series of 'what if' questions based on the trends you identified via the PESTEL exercise.

the steps here are:
- review the trends that could impact you
- identify the trends with the greatest potential for impact
- build the possible scenarios
- assess the impact of each scenario

#### futures funnel

basically, think about:
- the set of plausible futures
- the set of probable futures
- the set of preferred futures

And present them as a venn diagram. can act as a mini, less rigorous scenario planning  exercise

Could be useful to think about:
- internal
    - financial, org resources
    - current and future architecture
    - current and future product portfolio
- conceptual
    - correlations
    - causations
- external
    - potential futures
    - competitive trends
    - changes in consumer behavior


#### backcasting

aka "work backwards." the opposite of forecasting: starting with some tangible future, ask what needs to happen to make that a reality. repeat until you get to the present day.

- create a simple, tangible picture of the Beautiful Future. it has to be tangible and it should be clear once you’ve reached it
- hypothesize the prior state of the beautiful future
- repeat until you get to the current state
- check your work. run forward in time and make sure all the steps make sense



### chapter 4: industry context

SWOT

- Strengths (helpful, internal)
- Weaknesses (harmful, internal)
- Opportunities (helpful external)
- Threats (harmful, external)


It can be useful to create a matrix to house the results of your analysis


#### Porter's 5 forces

- threat of new entrants
- ease of substitution
- bargaining power of consumers
- bargaining power of suppliers
- industry rivalry

can be useful to present this, one per slide, with a traffic light green / yellow / red based on your results


#### Ansoff growth matrix

- market penetration (current market, current products)
- market development (current products, new market)
- product development (new market, new products)
- diversification (current market, new products)

Useful to use a 2x2 matrix with the results here


### chapter 5: corporate context 

#### stakeholder alignment

- to get stuff done, you have to havre alignment and buy in from
    - leaders (people who you work for)
    - the people who will execute it (your reports)
    - your colleagues, who can undermine or ignore you
- make list of everyone, put their names titles, and orgs
- rate each for
    - impact (the degree to which the strategy will impact the person)
    - influence (how important this person’s support is)
- based on influence and impact, sort into four buckets:
    - monitor - low impact, low influence
    - maintain confident - low impact, high influence
    - keep informed - high impact, low influence
    - collaborate - high impact, high influence


#### RACI

Responsible, accountable, consulted, informed

Number one mistake is to assign more than one person as accountable
If we do this, rethink the line item, maybe break it into two


#### Growth-share matrix

Another 2x2’er:: market share x market growth:

- cash cows: high market share, low market growth
- dogs: low market share, low growth
- question marks: low share, high growth
- stars: high share, high growth

Useful for managing portfolios of projects.


#### Core / Innovation Wave

Can be useful when considering a set of future project and you aren’t sure which ones to pursue. Useful for Ansoff growth matrix and Investment Map. Can be used on multiple 'levels' of the org (project planing, portfolio management, etc.) Another 2x2’er:

- proximity to the core: how close the project / product / feature etc. is to your main business or applications
- innovation: does this already exists already, or dos it need modification, or it is totally new?

make a plot like this:



#### Investment map

- List the items in your portfolio and any new ideas / initiatives
- Score them occurring to how difficult they would be and how ready the market/customers are for each
- generate a 2x2 matrix

- Very hard, ready now: proof of concept
- very easy, ready now: invest now
- very hard, not ready: don’t invest
- very easy, not ready: monitor

Works well with core/innovation map and growth / share matrix.


### chapter 6: department context

There was a lot of content in here, but honestly it didn’t flow together super well.

Good example: https://www.nasa.gov/sites/default/files/files/IRM_SP_2014.pdf


#### principle, tools, and practices

Idea here is that you want all these to be made explicit and in alignment. principles are foundations of a systems of beliefs. they might represent tradeoffs you’re making or bets you’re making about how to approach a problem. they might be things like 'well-managed' or 'data as an asset', or 'design for failure'. 

practices are the things that people do every day. and tools are the things that people use as part of carrying out the practices.

there’s a long section in here about process posture maps and current /future state operating models that were a bit abstract to me. I think the key thing is listing out all your processes in a slick slide or set of slides, and for each, determining whether to 

- start
- continue
- invest
- assess
- revise

Put the key gaps in a 'current vs future operating model' slide highlighting areas where change needs to happen in your processes.

finally, connect principles to practices and tools in a snaky diagram. very visual, and makes it very clear if your principles, e.g., are not really being supported by any meaningful processes.


#### Application portfolio management

Again, there was a lot here. This is a broad framework for keeping track of projects or initiatives in your org.

Some outputs of the process:

Another 2x2’er with dimensions (a) technical risk and (b) important & alignment:

- low risk, low importance: tolerate
- low risk, high importance: grow / evolve / maintain
- high risk, low importance: retire
- high risk, high importance: reengineer / modernize / replace


It can also be useful to create a project heap map, esp. if you are new to the org. Axes are project quality and value to the business:



### chapter 7: approach plans

#### 30 second answer

- map an outline of three bullets in your head
- add three reasons / characteristics with high-level statements
- stop talking

the boss usually wants to know
- the project status
- do they need to provide any help
- your recommendation on some proposed action


#### rented brain

basically, pretend you are a consultant at work. tell bad news if there’s bad news to tell. be honest with your recommendations.


#### ars rhetorica

- logos
- ethos
- pathos

your argument might include
- using deductive and inductive reasoning
- stating your hypothesis and why you have that hypothesis 
- stating your method to proceed in validating the hypothesis
- what metrics you’ll measure to understand whether your hypothesis is valid
- probabilities and ranges


#### fait accompli

this pattern is: if you are making a big pitch that will requires lots of buy-in, talk to everyone individually first and make sure they are on board with it. incorporate their feedback. then in the meeting, name drop their name and how they helped with part X. 


#### dramatic arc

- establish the status quo
- create an inciting incident. point out what happens, and be specific, if we stay with the status quo
- the plan: the fix things, present your recommendation. show what changes you expect across people, processes, and technology. who will be involved, what will they do, what processes need changing, etc.
- shock and awe: what does the world look like after your plan? how will you measure success? what structure will you put in place to report back on what happened (e.g., a steering committee make up of stakeholders)


#### deconstruction

often, we find ourselves solving the same problem over and over again. when solving a problem, think at three levels:

- the local problem
- the category that this problem is in
- the associations in which this problem arise in other contexts

he argues that there are three causes of problems in tech orgs:

- lazy people
- people who don’t think about how they think about their work
- misunderstandings of semiotics (people talking about different things, not defining their terms, etc)

the goal should be to look at a problem and think, 'how can i never have this problem, or a related problem, ever again': rather than solving it, how do we just not have this problem?


	

### chapter 8: templates

#### one-slider

#### use-case map
- customer outcome
- fatures
- data components
- system components
- customer success measures


#### on estimating things
- realize that good estimates are themselves projects
- give ranges to express uncertainty
- get clarity on whether a rough, refined, or realistic estimate is needed. the latter may take weeks
- state the assumptions you used


### chapter 9: decks

#### ghost deck

aka an outline:
- write the outline outside of the deck software
- write only the headline of each slide. read them together. stay high level. make sure they make sense.
- do the headlines form a dramatic structure?
- figure out what supports each headline. what data / evidence do you need to show for each?


#### the ask deck

- first slide is written last. put the ask at the top of the slide. the bullet points are
    - the current state is X, Y, Z
    - therefore, do A
    - there are milestones along the way we’ll use to check in
    - this will take X duration, cost Y money, and require Z teams
    - there’s the end state at the end of all this
- ideally, if an exec doesn’t want details, they should be able to look at that single slide, know everything they need to know, and give sign-off



## good quotes:

If you're not making statements that someone could reasonly argue with, you're not making a meaningful or impactful statement – you're not making a choice and putting a steak in the ground to forge a future

"you are always building a system"

"there’s never enough time to do it right, but there’s somehow always enough time to do it over"

"you’re never quite solving a problem. You’re only trading it for when you’d rather have."

"strategy is the art of creating power.” -lawrence freedman




## appendix: characteristics of systems

characteristics of systems:
- scalability
- fitness to purpose
- portability
- exentisability
- availability
- monitor ability
- maintainability
- resilience
- security
- audibility
- performance
- testability
- elegance

Principles:
- hide details behind an interface
- apply the principle of least knowledge
- create a strong separation of concerns
- ensure loose coupling
- isolate what changes independently
- look for opportunities for reuse
- explicitly manage risk

SOLID:
- single responsibility: a class should have one job
- open-closed: open for extension, closed for modification
- Liskov sub principle: objects of a derived class should be substitutable for a parent class
- interface segregation: a client should not be forced to implement an interface it doesn’t use, or depend on methods it doesn’t use
- dependency inversion principle: things must depend on abstractions, not concretions
