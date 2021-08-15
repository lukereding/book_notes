# models for thinking and problem-solving

### what is the goal / problem

This seems really simple but violating this simple idea is routine. Whenever you're thinking through something, make sure ou know what the exact problem is you're solving for. I've found it's quite typical for the problem to be ill-defined and nebulous. You can't solve a problem if the problem isn't clear.

It's often useful to take a step back. Think about what the goal is, what you are trying to accomplish. Don't think about specific tools or methodologies. Often we presuppose that we using tool X or approach Y will mean we achieve our goals, but this is often not the case.

An example might be: a client for a streaming video service wants you to recommend the next video to play for each customer after they watch a video. What's the goal here? What are we optimizing for? It's still nebulous. Maybe after some back and forth you realize that client wants people to _watch_ the next video you suggest, not just click on it. There are people that might jump to suggesting specific recommender-based approaches. But I think that's the wrong approach. Because once you implement your solution, you need to understand how to evaluate it. Which mean you'll need to do some kind of A/B testing or experimentation. And you'll probably want to compare any fancier approach to some simple heuristics to see how they perform, like suggesting the next episode, or suggesting the most popular show they haven't watched. You'll need a system that could route traffic via for these different solutions. As you see how the heuristic solutions perform, think about what the results mean. Often this whole process is a means of understanding the problem. In this example, the implementation of the recommend system, if it ends up being necessary, is such a small step in a larger process of understanding the problem and figuring out the smallest solution to the problem that might work.

### what do I need to know

Most of the time, we're happy creating a story in our heads to explain data we see or a pattern we observe. In doing this, we only consider a single world or a small subset of worlds: those that happen to pop into our minds to explain the pattern.

A more robust way of understanding the world is to ask, before looking at the data: What would I need to know to be confident about answering this question? Then look at the data you have. Doing this is a guard against forming a story that seems plausible to you but is, in reality, based on a smalll subset of information you need to truly understand what's going on.  Alternative blindness, cherry-picking, and survivorship bias are all highly related to this idea.

### imagine the future

If we did X, what do you think would happen? Try to imagine the future. Useful for thinking about second- and third-order effects.

For example, what impact does rent control have on afforadable housing? Looking at the first-order effects, rent control seems like a good thing by making housing more affordable. But imagine what happens next. Rent control makes it less attractive for developers to build apartments, since their profits are limited by the rent control. As a result, fewer apartment buildings are built and there are fewer apartments to go around. The apartments to be had are afforadable, but there are very few of them. Developers might turn to building condos or other types of housing instead that are exempt from rent control. The result may be an exacerbation of the affordable housing crisis. This is also an example where thinking in systems--thinking about all the components that contribute to a problem--helps us gain more insight.

### work backwards

A related idea that can help clarify thinking and improve focus is to ask yourself: what's the future I'm building towards? Can I work backwards from the to figure out what I need to do now?

### what's the null hypothesis?

There are plenty of cognitive biases that masquerade by different names (e.g. survivorship bias, failure to consider base rates, self-selection bias, story bias) but at their core is the failure to consider the null hypothesis. Whenever you come across something that looks interesting or out-of-the-ordinary, or is presented to you as such, always ask yourself what you'd expect to happen if nothing interesting is happening in reality.

### commit to and revise your mental models

The only way to learn about how the world works is to (a) form a hypothesis, (b) observe, (c) when something violates your hypothesis, it means your model is wrong and needs updating, so (d) update it and continue the process. Another way of thinking about this is to identify gaps between what happens in the world and what you think should have happened.

The difficulty in applying this idea lies in its implicit requirement to interpret the world without bias. It is easy to see the world in a way you want to see it. You have to change your thinking from wanting to be right and internally consistent to having a true interest in understanding how the world works.

### when you find a difference between what you expect and what you observe

Ask yourself:

- Are my assumptions wrong?
- Are my data flawed?
- Or my intuition flawed?

### is the sample biased?

When evaluating data, always ask yourself whether the sample is unbiased or not. In most cases, the interesting data we hear about come from biased samples, making the inferences we make based on the data suspect or severly limiting.

### root cause analysis / systems thinking

To me, these are closely related. Once you ask _why_ five times, you tend to overcover the broader system. When you do this, it's useful to diagram all the resulting pieces of your problem and the interactions between them. Systems thinking and root cause analysis are especially powerful because they force you to think about the broader system or context in which a problem occurs instead of one isolated component.

### segment

I continue to find [Simpson's paradox](https://en.wikipedia.org/wiki/Simpson%27s_paradox) disturbing. If we really want to understand patterns we see in data, we often need to segment them to understand the extent to which the patterns hold true in each group.

### refuse all-or-nothing thinking

The world exists in greys. But taking an all-or-nothing approach to things--someone is evil or good, the research paper is garbage or valuable--denies you of the richness of the world and the truth. All-or-nothing thinking is a heuristic. It's convenient and simple, but it puts you further from an complete understanding of the idea, event, or context you're trying to understand.

### expected value calculations / sensitivity analysis / net present value

### weight opinions by credibility

### supply and demand

Many phenomena can be understand simply by asking questions about supply and demand.

### facts vs. generalizations vs. assumptions

It's important to be able to tease about, in any argument or opinion: what are the facts? what are the generalizations? what are the assumptions?

### positive and negative controls

### do the opposite

If you're stuck thinking about how to solve a problem, it can be helpful to _invert_ and think about ways to solve the opposite problem, then do the opposite.

## specific techniques / models

### what will the effects of this be in 5 min, 5 months, and 5 years?

#### sequential anaylsis

Be able to answer:

1. What is the problem?
2. Where does it lie? (i.e. what is the system or the process that produces the problem?)
3. Why does it exist?
4. What could we do about it?
5. What should we do about it? You should be able to visualize the world with your recommendation in place.


#### SWOT

- strengths
- weaknesses
- oppurtunities
- threats

#### policy analysis

__Effects__
1. What are the intended effects?
2. What are the unintended effects?
3. How will the policy affect different sub-populations / groups?

__Implementation__
4. What's the cost?
5. How feasible is it?
6. Do the stakeholders view the policy as acceptable?


#### logic trees

[__Logic trees__](https://en.wikipedia.org/wiki/Issue_tree) can be a useful way of decomposing a problem into it's component parts and identifying the lower-level issues that contribute to a problem.
