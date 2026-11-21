# engineering a safer world
Leveson

I really enjoyed this book, mostly because it fuses two things I like to think about: systems and risk. The book is similar to others I've read, notably _drift into failure_, but more structured and academic.

### chapter 1: why do we need something different?

Makes the argument that the types of systems that commonly get built together have different characteristics than those of yore:

- faster tech changes
- changing nature of accidents
- reduced ability to learn from experience
- increased complexity and coupling
  - interesting taxonomy here between interactive complexity, decompositional complexity, nonlinear complexity
  - "complexity can be defined as intellectual unmanageability"
- decrease tolerance for single accidents
- complex relationships between humans and automation
  - "many recent accidents that have been blamed on operator error could more accurately be labeled as resulting from flaws in the environment in which they operate. 

### chapter 2: questioning the foundations of traditional safety engineering 

This is very similar in spirit to Dekker's arguments against the 'legacy of newton and descartes' and I found it particularly satisfying. She dismantles many of the traditional assumptions taken for granted about safety engineering:

- confusing safety with reliability
  - she argues that safety and reliability are orthogonal: something can be reliably unsafe, or safely unreliable
  - in particular, many accidents in systems take place from _interactions_ between components, not because a component failed
  - "Button-up decentralized decision making can lead—and has led—to major accidents in complex sociotechnical systems. Each local decision may be 'correct' in the limited context in which it was made but lead to an accident when the independent decisions and organizational behaviors interact in dysfunctional ways." <= very similar idea to _drift into failure_
- modeling accident causation as event chains
  - "all models are abstractions; they simplify the thing being modeled by abstracting away what I assumed to be irrelevant details and focusing on the features of the phenomenon that are judged to be the most relevant selecting some factors is relevant and others as irrelevant is in most cases, arbitrary and entirely the choice of the modeller."
  - she argues that simple causality models are attractive because they are simple, and not because they are correct
  - event chain models cannot account for nonlinear relationships that exist in many systems
  - event chain models tend to encourage finding a single "root cause." in the context of a system, a single root cause is an illusion. practically, she argues that often finding a root cause that is "politically acceptable" is the most likely outcome.
  - event chain models are also extremely limiting, because they often "omit causal factors that cannot be excluded in the event chain," like the broader context of the event or other pressures or constraints that influence the event but doesn't represent distinct events: "event-based models are poor at representing systemic accident factors such as structural deficiencies and organization, management, decision-making, and flaws in the safety culture of the company or industry"
  - "instead, degradation in the safety margin occurred overtime and without any particular single decision to do so, but simply as a series of decisions that moved the plant slow slowly towards a situation where any slight error would lead to a major accident." - sounds a lot like drift towards failure
- limitations of probabilistic risk assessment (PRA)
  - this idea is basically what's advocated for in _the failure of risk management_
  - she makes the point that most of these analyses assume independence, which is rare in systems and when an accident occurs (I'd add: in a crisis, all correlations go to 1). "most accidents in wild design systems involve two or more low probability events occurring in the worst possible combination when people attempt to predict system risk they explicitly or implicitly multiply events with low probability – assuming independence – and come out with an impossibly small number when in fact, the events are dependent"
  - PRA usually discounts / doesn't cleanly allow for component interaction accidents 
  - PRA is usually grounded using past data, which is likely unrepresentative of the true future-looking risk
- the role of operators in accidents
  - she argues that "it is...very difficult to separate system design error from operator error," though operator error is found to be the cause of 70-80% of accidents
  - "providing feedback and allowing for experimentation in system design, then is critical and allowing operators to optimize their control ability." She argues that automation can be counter-productive, by preventing operators from establishing a correct mental model they can use when things go wrong
  - "it is difficult – if not impossible – for any individual to judge the safety of their decisions when is dependent on the decisions made by other people in other departments and organizations"
- the role of software in accidents
  - she argues that _incorrectly specified intent_ is the cause of software accidents, 
  - "the extra communication step between engineer and the software developer is the source of the most serious problems with software today... Most errors found in operational software can be traced to requirements flaws"
  - reliability != safety 
  - "nearly all the series accidents in which software has been involved in the past 20 years can be traced to require requirements flaws not coding errors. The requirements may reflect incomplete or wrong assumptions."
  - biggest failures occur when no one understands what the software should do and what it shouldn't do
- static vs. dynamic view of systems
  - accidents result in systems becoming less safe over time -- she is basically grokking Dekker here in _drift to failure_
- there's some very interesting things in here about blame and how if the interest it to understand the system to better improve it, blame is not a productive use of time; a shift from _causes_ to _reasons_ is required 


### chapter 3: systems theory and its relationship to safety

- 'safety then can be viewed as a control problem'
- Fig. 3.2 in the book is clarifying: a controller controls actuators which have some effect on the process we care about, in addition to other things we can't control. sensors measure the environment and 'report back' to the controller. very similar to the framework provided by a multi-armed bandit.