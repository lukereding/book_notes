# the ten equations that rule the world

sumpter


This was a enjoyable pop-y math book. Some things I want to remember:

- Use Bayes more often. Can really be useful to prevent 'overfitting' to individual changes or observations, which I'm guilty of
- I also like the form of Bayes he used and the notation. There are models--things we thing underpin the world, true truths--and data, things we observe. The form is then P(M | D) = P(D | M)P(M) / [P(D | M)P(M) + P(D | not-M)P(not-M)]
- Often when we read seemingly incredible things that make sense to us, or when we hear about a new article that makes a claim that seems supported by data, we are often forgetting the second term in the denominator. In general, when you hear something like that: think about all the other hypotheses that could also explain the data
- A powerful model to use when forecasting or otherwise thinking about the future: imagine a library of possible futures in your brain. 'Assign' a likelihood of each happening, and update these likelihood using Bayes when new data comes in
- State your assumptions -- often this is really difficult because we tend to make a bunch of implicit assumptions
- Think about separating information you absorb into three categories: models / hypotheses, data, and nonsense. the idea being that there's a lot of stuff we encounter that's non-verifiable nonsense that's just noise
- the reward equation explains a lot of behavior and explore/exploit dynamics in animals: Q_t+1 = (1 - a)Q_t + aR_t, where Q_t is the estimated value at time t (which converges to the true actual value), R_t is the reward at time t, and a is the learning rate which 'tunes' explore / exploit. Also depends on the Markov assumption.
- The success or failure of any model is largely dependent on a modeler's ability to understand which parts of the problem to simplify, and which assumptions are okay to make