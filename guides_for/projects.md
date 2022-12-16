# projects

My running list of various things to keep in mind while managing projects.

## Checklist for projects

This should be

- written down
- somewhere public where people can refer to it

Here are the ingredients you need to consider:

- Goal
	- What the purpose of the project?
	- This should be tactical what you’re trying to accomplish, but also provide the _why_ and how it fits into the bigger picture of the organization or team
- Functional / non-functional requirements, and what’s out of scope
	- Functional requirements = how you know you’re done with the project. These are hard lines in the sand
	- Non-functional requirements. Stuff you want to maximize and minimize in the process, but not necessarily hard requirements. For example, you might want to reduce costs as much as possible, but you don’t have a clear line in the sand for a cost target to hit. Or maybe there’s a clear requirement on load (e.g., able to return scores on 1M accounts in an hour), but solutions that are able to handle greater load should still be judged as better than those that barely hit the functional load requirement
	- What’s out of scope is important because it clearly defines what you _won’t_ do and gives you clear permission to say 'no'
- Timelines / milestones
	- You need a broad timeline and check-ins along the way
	- Multiply initial estimates by 2-3 to get a more realistic timeline
-  Risks and mitigations
	-  Early on at the project initiation phase, you should be probing for risks wherever you can. Finding stuff that can go wrong early is great: finding these things out later is much, much more costly
	-  During project initiation, you want to meet with all stakeholders and people you have a dependency on. You want to ask them about what could go wrong, risks they see, things that keep them up at night. Tools here include asking lots of open-ended questions to get at unknown unknowns and using premortems
	-  For each risk, identify at least 3 or 4 possible mitigations
-  Dependencies
	-  This is a special case of a 'risk' but it’s so important it’s worth calling out separately
	-  If there are teams / people you depend on to deliver your work, you need to make these dependencies really clear
	-  You also need to make it clear to (a) your stakeholders and (b) these dependencies _how_ you’re going to facilitate alignment, escalate when a team might not pull through, and generally manage the dependency on the other team
-  Stakeholders
	-  You need a list of your key stakeholders. These might change, but it needs to be super clear to everyone on the team who the customer is and what they care about
-  Meetings and update cadence
	-  You need some way of sharing out updates, progress, blockers, etc. You also need touchpoint so stakeholders are never wondering 'I wonder what’s going on with team X'. 
	-  In your project doc, you should be clear about what meetings existence to facilitate alignment and problem-solving, the goals of each meeting, and the intended audience
		-  You might have some internal meetings every week where the goal is to share updates and blockers, or to problem-solve within the team
		-  Other meetings might be more formal share-out meetings with stakeholders that occur on a regular cadence
-  List of team members and responsibilities
	-  A RACI is a good tool to use here
	-  This helps set expectations and makes it clear what everyone on the team is responsible for


### How you get there

- idea generation / generate buy in internally.
- shop it around
	- go to each stakeholder
	- open-ended questions / unknown unknowns
	- probe for risks
- alignment meetings and sign off
	- these should be a piece of cake if you’ve already talked to every individually

## Other considerations

#### Do you really need to solve that problem?

I've found that often people are all too happy to start a new project--maybe they just got a promotion or someone's budget was increased--without clearly knowing what they want out of it. The simplest things are often the hardest to pin down, in this case: what's the problem we're trying to solve? Seems very simple, but I've been on many projects where the goal of the project is assumed, or its never codified and is allowed to bend and warp over time. Such situations can't lead to success because no one knows what success looks like.

Generating a document with the elements listed above is an antidote to this anti-pattern.

#### Things will take longer than you think they will

Hofstadter's law; principle of multiplying estimates by 2-3 to get at a more reasonable estimate of timing

#### Allocate roughly equal time to design, implementation, and testing for tech products

#### Understand the customer

If you’ve followed the suggestions above for your project doc, you should have this one covered, because a core stakeholder (esp. for internal products) is the end user of what you’re building. If the end user is a broad base of people and not a team or business unit, this will be harder. Understand how the product is used. Ask the end users questions but do not simply do what they tell you to do. You want to understand the users __goals__ and their __latent needs__, not just the goals or products or features they _think_ they need.

#### Why projects fail

This (rough) list was presented to us during TVL; I thought it's inclusion here was useful:

- not enough time is spent on planing up front. solution: create the project document listed above
- the client / customer / stakeholder doesn't get back to you. solution: make sure you have a clear cadence for updates and make sure you’re actually solving the right problem
- team members have different ideas about how to accomplish a task. solution: hold working sessions to facilitate problem-solving across the team
- work is not appropriately distributed. but clear with roles and responsibilities up front and shift around work as things change
- the team leader doesn't get updates from team members. solution: hold regular project check-ins
- scope is not clearly defined. solution: create the project document above
- outcome is not clearly defined. solution: create the project document above

