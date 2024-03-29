# Making things happen
Scott Berkun


This was a great read. Lots of interesting thoughts and good advice.

This book is all about project management: 

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

Lame visions speculate, avoid taking an opinion, and avoid the possibility of being wrong. 

**Visions should be visual**. You should evoke an image in the reader's mind of the end service / product and how it contributes to a customer's goals. If the end result can't be visualized, the vision isn't clear.


## figuring out what to do

I.e., the 'flare' in 'flare and focus'

Requirements are critical. They focus by eliminating possibilities and stimulates designers to ask more questions to refine the requirements.

There are bad ideas. The space of possible bad ideas is generally much larger than the space of ideas that actually solve the problem / satisfy requirements. 

> the real craft of problem-solving and creative thinking is knowing which constraints to use or ignore and when to do so (p. 98)

> Big, radical ideas are rarely needed to succeed. More often, it's a handful of basic, solid, good idea--applied correctly--that are needed. (p. 98)

Well said.

There's a large section in here about the importance of settling on a clear question. He argues that most people in tech have lots of interesting knowledge that they're more than happy to share, regardless of whether it's applicable to the problem at hand. Good questions are focusing and they draw people to something important.

> ...good questions identify an essential Element of the problem (or solution)-bypassing all of the secondary and nonessential information-and create a space for an answer to be born (p 100)

He claims and is powerful question and all is project management, creative thinking, or problem-solving is:

__What problem are we trying to solve?__

I've thought about this a lot and found it super clarifying. I use it regularly, thought I don't think others have found it as clarifying as I have.

> Creativity is just connecting things (quote from Jobs)

Some ideas for idea generation:

- Yes, and... - i.e., keep things moving
- Be committed to what you say / no half-assing
- No blocking questions


## what to do with ideas once you have them

i.e., the 'focus' in 'flare and focus'

In general smart teams figure out requirements and dependencies early on, but it may not be possible for complex projects. You'll often find yourself taking two steps forward, one step back. You'll find that you make a decision, but you won't see all the issues and problems that arise from that decision. I think the only way to figure out what all these issues are is to make a decision and see where it takes you.

It's useful to have a series of milestones or check-in's. During the specification process, i.e., the focus part of design, you might milestones for when you're down to to three alternatives or two, or have the final specifications in place.

Prototypes are great. They take everything that's been learned and apply it to the problem without taking on the risk so for implementation. They allow the team to improve their thinking before they commit to a plan.

You should try a different ideas early on in the process, to see which ones work and which ones don't. It also helps to make each idea concrete and ensures everyone understands each idea the same way. (lots of connections here to _creative confidence_.)

## how to make good decisions

The first part is to determine the significance of the decision of hand. Questions to ask:

- What problem is at the core of the decision?
- How long with this decision impact the project?
- If you're wrong, what's the impact or cost?
- Has this sort of decision been made before?
- Who's the expert?
- Who's approval / feedback do we need?
  
Differentiates between singular and comparative evaluation. In the former, you're basically using a threshold to make a decision. In the latter you're comparing all your options along some criteria of interest. To get the best solution, you usually require comparative evaluation.

He recommends just listing out all the potential options and list the pros and cons for each. Some nuance:

- Always include a 'do nothing' option
- How do you know what you think you know?
- Ask tough questions
- Consider hybrid choices

He knows that having more information doesn't necessarily make for a better decision. Information can help, but only so much.

> The best decisions for projects are often unpopular, or upset or disappoint some important people on the team, and will make you an easy target for Blaine if things go wrong.

This ^ aligns well with strategies and make clear (and tough) tradeoffs in _an elegant puzzle_. 

Importantly, good decisions can have bad outcomes. In most cases, you're making a decision with incomplete information, and there's some still stochasitcity involved. You can make a decision that has, e.g., a positive expected value, but still lose money on that one decision.
## communication and relationships

At it's simplest, there are five basic states of communication. Communication is only successful if it reaches the third, if not forth and fifth states:
1. Transmitted
2. Received
3. **Understood**
4. Agreed
5. Converted into useful action

That is, sending an email to someone is not an act of communication unless what you were trying to communicate was understand, and hopefully, roused some action on the part of the recipient.

Common communication problems:

- Assumptions. Good communicators clarity assumptions at key points, such as when commitments are made
- Lack of clarity. "It's not what you say, it's what they hear." It doesn't matter how eloquent you are, if it isn't clear to them it doesn't matter.
- Not listening
- Blame
- Problem mismatch - are you talking about the same thing? Is there an unresolved issue somewhere?

Stephen Covey: " The cause of almost all relationship difficulties is rooted in conflicting or ambiguous expectations around roles or goals"

Getting people's best work:
- Great leaders never force anyone to do anything
- Listen to your people--take suggestions seriously
- If the vision is strong, the work interesting, and the people get along, there's little need to demand anything
- Clear roadblocks
- Inspire people -- remind them how great it is to work on the sort of problems you're working on, what impact you're having, etc.
- Remind them of the project goals
- Ask

## how not to annoy people

Three activities with the greatest odds of annoying people are email, meetings, and team processes.

Why people get annoyed:
- Assuming they're an idiot
- Lack of trust
- Wasting time
- Manage without respect
- Make them listen or read stupid things

The trick in creating good processes is to understand two things: what makes projects and team successful in general, and what makes the current project and team different from others. Do you want to account for the culture, personality, and habits of the current team that you're working with.

Good process:

- accelerates progress
- prevents problem
- make important actions visible and measurable


Costs of a process: determined by time to design to process (DT), time to learn it (LT), the actual time required by the process (AT), and how often it's done (N):

cost = DT + LT + (AT*N)

Benefits are based on cost of failures the process avoids (FC), the probability those failures occur (FP) without the process, and how many unit of time T are in the project:

benefit = (FC * FP) * T

Process value = (FC * FP) * T - (DT + LT + (AT*N))

To roll out a process:
- Identify the best proposal. MAke sure it's solving the core problem you care about
- Identify a low-risk part of the project to test it out on. Is possible, pick a team or person who's interested in the new process. Align on desires effects and what will be measured.
- Implement to processs
- Set a time in the future to circle back and evaluate the process
- If it worked fine, roll out to the larger group

In cases where stupid process exists, a good tactic is to simply ignore it:

> I have a tendency to ignore distant, ambiguous, bureaucratic, organizational things that I don't understand. My theory is that I ignoring it, I force one of the two things to happen. Either the person responsible for the thing or contact me and ask why I didn't do it, giving me a chance to have a dialogue with him about why I should do it at it at all; or, as no one asks me why I didn't do it, then it can't possibly be that important

### email

Tips for writing good email:

- Be concise, simple, and direct. ("If I had more time, I'd write a shorter letter.") Really think about who is reading the email, their assumptions, what they already know, etc.
- Offer an action and a deadline
- Prioritize. Is everything in your email that important? Can you collect things into groups instead?
- Don't assume people read everything
- Avoid giving a play-by-play. It's rare that someone needs to know the sequence of events that led to something. **Make it possible for anyone to skim the first two lines and know immediately if it's important enough for them to read further.**

Awful email is long. It's hard to skim. It's poorly written, and it has many attachements.

### meetings

Your job is to facilitate. Sometimes, if people are going all over the place, to write down a list of the key issues, ask everyone if to affirm that these are the key issues, then go through them one at a time.

Pointers for facilitating:

- Establish a host position. Introduce people, clarify the agenda, begin the discussion
- Listen and reflect. If someone says something half-baked, help them develop the idea. Or if someone says something unclear, say "So Mike, what you're saying is < reclarify what Mike was trying to say >, is that right?" 
- Direct the conversation. If the conversation really starts to get off track, pull it back. If some people aren't talking much, ask for their thoughts.
- Know when the end the conversation. It's often useful to identify action items, DRIs, and intended results.
- Record stuff. Write stuff down. Document the discussion! What's important is that when the meeting is over, next steps and action items are clear and emailed out to the group

## what do to when things go wrong

- Calm down
- Evaluate the problem in relation to the project
- Calm down
- Get the right people in the room
- Explore alternatives
- Make the simplest plan
- Execute
- Debrief


### conflict resolution and management

- Find the point of unification. Two people, no matter how much they disagree, agree that somethings: the world is round the sky is blue the project needs to be on time. Find the important points of unification in agreement uses to starting any discussion you have
- Look for mutual intern. Frame things around interests, not adversarial positions. 
- Look for areas of compromise. Are there less important things you can cave on to show some goodwill?
- Know the alternatives. Always know what the cost is of walking away from the table without an agreement. 
- USe persuasion and argument. "the interests and desires of both parties are based on subjective opinions about the relative value of things. This means that if you can develop a true understanding of one parties feelings, you can possibly persuade them that one aspect of the situation is more (or less) desirable than they thought"

## interesting quotations that don't fit neatly into the above

> Project managers must be persuasive in getthing the team to strive for simplicity in the work they do, without minimizing the complexitites involved in writing good, reliable code

> Confusing processes with the goals is one of the great sins of management.

> Make good stuff happen

> The real craft of problem-solving and creative think you know in which constraints to use or ignore and when to do 

> The most powerful question in all of project management, creative thinking, and problem-solving is: what problem are you trying to solve?

> Creativity is just connecting things.