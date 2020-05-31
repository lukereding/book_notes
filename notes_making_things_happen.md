# _making thing happens_
Scott Berkun


This was a great read. Lots of interesting thoughts and good advice.

This book is all about project management : 

> leading the team in figuring out what the project is (panning, scheduling, and requirements gathers), shepherding the project through design and development work (communication, decision making, and mid-game strategy), and driving the project through completition (leadership, crisis management, and end-game strategy).


## schedules

Schedules have three purposes:

1. communicate committments about when things will be done

2. encourage folks to see their work as parts of a greater whole

3. provide a tool to track progress and break up work

The _rule of thirds_: break up the available time into thirds
    - design
    - implementation
    - testing

### why schedules fail

- most people are optimistic planners
- precision != accuracy
- think of a schedule as a probability
- estimating things is hard, esp. if the team or the work is new
- good estimates come from good designs and good engineers: the work should be clear and the people doing the work should have a clear idea of how to carry it out 
- Useful question to ask: "What questions can I answer that would make you more confident about giving an estimate?"
- Estimates should have confidence levels / probabilities
- Estimates depend on how well folks know the overall goals of the project

Common oversights include:

- not taking into account sick days / holidays / vacations etc.
- not making sure you're tracking to the schedule on a regular basis
- the team not feeling committment to the schedule
- were the goals of the project => specs / design plans clear enough to enable accurate estimates of how long things would take?
- did folks on the team feel like they could say _no_ to work that did not address one of the goals of the project?

Snowball effect: If you miss your first deadline, the probability you miss your second deadline skyrockets

### making schedules work

- Milestone length should make project volatility
- be optimisitc in vision and skeptical in the schedule
- plan checkpoints where features can be add/cut according the changing needs or information
- understand the team's familiarity with the project space
- take on risks early

## figuring out what to do

Simple way of thinking about things:
- requirements => what do we need to do?
- design / specs => how do we do di?
- implementation => do it

### the three perspectives

#### business

Focuses on P&L, costs, etc. Ask questions like:

- why is this project needed for our business?
- what unmet needs do our customers have?
- on what basis will customers buy this product / service?
- what will it cost?
- what won't we build so we can build this?
- how does this contribute to our long-term business goals?
- competitive analysis

#### tech

It's common that tech concerns win out and you build something that's technically interesting to the engineers but doesn't solve a problem customers care about. There's a bias towards the actual building of things as opposed to understanding how those things will help the business or a customer. 

Tech asks questions like:

- what does it need to do?
- how will it work?
- what technologies / architectures / etc. can we use?
- what knowledge / expertise does the team have?
- how much time will it take to build?

#### customer

The most important of the three perspectives. Tries to understand what customers want to do, how they currently do it, what changes or improvements would help them achieve their goals. Build from two sources: requests and research. Note that requests from customers are not the same as understanding a problem: a customer can request a feature that they think helps them, but the actual need the suggested fix is trying to solve might be solved for in a better / more straightforward way. 

This perspective asks questions like:

- what do people actually do?
- what problems do they face? where do they get stuck or frustrated?
- what do they want to be able to do but can't do?


### the interdisciplinary view

For every project, you have to understand things from these three perspectives: each perspective influences the others. 

A useful list of questions to ask:

- why does the project exist? why does it need to be done now?
- what kinds of customers are we serving? [think about coopers' personas.] what are they using our product / service for?
- do we have the technology and expertise needed to satisfy these problems
- what are the timelines for the next product release or launch?
- what are competitors doing?
[others listed on pg. 57]

### bad ways to decide what to do

- we'll do what we did last time
- we'll do what we forgot to do / didn't have time to do last time
- we'll do what a competitor is doing
- we'll build whatever is trendy
- we'll build it and people will use it as a result

### requirements

Once you figure out what to do, you'll want to put together a plan of action. This includes a **vision document** (see next chapter) and **requirements**.

Make problem statements. These are 1-2 sentences about an end-user or specific issue.. Problem statements get converted into features / scenarios. Each scenario describes what the customer will be able to do as a result of the project. These statements should be a pretty clear distillation of your customer research / what you've learned about your customers during the planning phase. 

## writing the vision

Documenting the high-level goals of the projects is important:

- makes the goals clear to everyone
- offloads details so you don't have to retain them in your head
- provides a point of agreement for the future

### qualities of good visions

1. Simplifying. Should provide concise answers to basic questions about the project be a tool the team uses to make decisions. Should make priorities and boundaries clear.

2. Intentional / goal- driven

3. Consolidated. Arguments and research behind the plan shouldn't be present in the main body is the vision doc. You could include these in supplementary materials if you want. 

4. Inspirational. Make sure it's clear the project is solving a specific real-world problem and not a technological one.

5. Memorable.

### key points to cover

- one-sentence articulation of what this project does
- how does this project contribute to the organization's goals?
- what scenarios / features are both (1) essential and (2) desired for the product?
- who are the customers?
- who are the stakeholders
- why will customers buy this thing
- who are the competitors
- how is this not a technology in search of a problem?
- what is out of scope?
- what are some likely reasons this project will fail, and how are those risks being minimized?
- are there other parts of the company that are depending on this project?

- should be as concise as possible
- should be authored by a single person, not by committee

Lame vision speculate, avoid taking an opinion, and avoid the possibility of being wrong. 

**Visions should be visual**. You should evoke an image in the reader's mind of the end service / product and how it contributes to a customer's goals. If the end result can't be visualized, the vision isn't clear.




## interesting quotations that don't fit neatly into the above

> Project managers must be persuasive in getthing the team to strive for simplicity in the work they do, without minimizing the complexitites involved in writing good, reliable code

> Confusing processes with the goals is one of the great sins of management.

> Make good stuff happen
