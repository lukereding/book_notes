# articulating design decisions

greever


this book is really about improving stakeholder interactions. the entire book is centered around the idea of a design review for capital-D Designer pixel-pushers, but the themes are applicable in any sort of scenario where you're managing stakeholders and have to deal with you doing a ton of work and take sometimes disorienting feedback from important people.


#### chapter 1

- He argues that great designers are greater communicators: this is what sets apart good from great, not raw design talent
- Every design needs to:
  - Solve a problem. You need to constantly ask yourself, _what problem am I trying to solve with this?_
  - Be easy for users
  - Enjoy support by stakeholders. Without this, you'll end up having a bunch of the same conversations over and over. To gain support, we have to explain why our proposed option _is better than alternatives_
- To make sure we hit all the points above, when we communicate our decisions, we need to answer the questions:
  - What problem does it solve?
  - How does it affect the user?
  - Why is it better than alternatives?

#### chapter 2: stakeholders

- the single most important thing you can do to improve communication between you and your stakeholders is to improve your relationships with them
- **ultimately, our jobs are to learn how to make our stakeholders successful**
- (a lot of this chapter is on building empathy wih your stakeholders and trying to see things through their lens)
- In cases where you find yourself butting heads over and over, it's likely that the goals / assumptions differ between two and the other person; address these head on:
  - what's your opinion on this project?
  - how does the project affect your job?
  - what's your priority for this project?
- a lot of this chapter is about getting the other person to talk to better understand what's going on in their world and what's important to them
- think carefully about who your stakeholders are and the things they care about; in general, an exec will have a different perspective than an engineer or a project manager


#### chapter 3: design the meeting

- a very useful framework for starting meetings, especially with busy people who context switch a lot:
  - state the goal. this is where you make sure it's crystal clear to everyone _what problem you're solving_
  - summarize the last meeting
  - show a timeline
  - specify the feedback you need
  - state the goal, again
- you need to _remove distractions_: you want people to be focused on what you say and not distracted by stuff like crazy colors or incorrect grammar
- anticipate their reactions
  - ahead of time, think about
    - what each person cares about the most
    - what their personal goals for the project are
    - what you know they want or don't want
  - write down any objections you expect _ahead of time_, craft a response, and rehearse the response
- create alternatives
- know who's in the room with you
  - you should know who else will be there to back you up; you can coordinate this ahead of time

#### chapter 4: listen

- this chapter is literally about listening to your stakeholders when they give you feedback during a meeting
- a lot of this is about _letting them talk_, even if they're saying crazy stuff, let them talk, let them say what they need to say. takes notes during this and let them see that you're taking notes
  - in the process, they might refine their thoughts
  - it gives them confidence they were understood
  - it demonstrates that you value what they're saying
- there's a lot in here about taking notes and writing down _why_ certain options where considered off-the-table or not persued
- when you're trying to clarify their feedback, **you can use these questions to get them to talk more** and explain themselves:
  - what problem are you trying to solve?
  - what are the advantages of doing it this way?
  - what do you suggest?
  - how will this affect our goals?
  - where have you seen this before?
- repeat and rephrase
  - repeat what they said and say it differently
  - common antipattern: the stakeholder says they 'like' this approach better than another approach. when that happens, _rephrasde in terms of effectiveness to achieving the goals_. E.g., "I like the idea of consuming from a low latency data store, that feels more appropriate to me" -> "I understand you're advocating for low latency retrieval; can you help me understand how that furthers our goal of X?"
  - i.e., a personal preference is not a good reason to execute a design decision


#### chapter 5: mindset

- give up control: realize that in a lot of cases, the final result is out of our control
- **part of your role is giving stakeholders the tools and vocabulary they need to go represent our work to someone else**
- anytime you think, "they are just wrong; I am right": tread lightly, check your ego
- **lead with a yes**
  - in responding to stakeholders, always lead with a yes
  - if you agree with the problem and not the solution, you can say: "yes, I agree that we need to reconsider X" or "yes, I agree with it's really important to get Y right"
  - "yes, and <insert tradeoff here>". you can use "yes and" to get a stakeholder to see the tradeoff they'd be forced to make. e.g., "yes we can do that, and the launch will be delayed by 10 weeks" or "yes, we can go down that route, and we'll need an extra three people to make it happen"
  - "leading with a yes is about reminding people of the areas where we agree, before we get to the parts where we don't"
  - other examples
    - "yes, that's a good point"
    - "yes, thank for for sharing that perspective"
    - "yes, I agree we need to solve this"
    - "yes, there are definitely some ways we can improve this"
- again, **don't focus on what you like; focus on what is effective in achieving the desired goals**
- "thank, repeat, prepare" when responding
  - thank them for their feedback
  - repeat what they said
  - tell them you're going to respond to their feedback, and how
  - examples:
    - "thanks for sharing your feedback. I appreciate the opportunity to go through all of this with you because it's important for us to be on the same page. I'd like to go back over everything you said because there are some important points where you need to be aware of our decisions and more detail, and it will help you to see how we're approaching this problem."
    - "thanks for sharing your thoughts with us about this project. Your insights are really valuable, and I appreciate you going through all that with us. I'm going to go back through all of your points so that we can discuss then, but I'd like you to understand how we came to these conclusions first..."


#### chapter 6: form a response