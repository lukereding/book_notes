# superforecasting

Tetlock and Gardner

An entertaining and interesting read. 

Some random notes and thoughts:

A lot of this was applicable to machine learning. For example, in his prediction tournaments, the best way to pool experts to form an ultimate estimate was to take a weighted average of all predictions, but weight the votes by past performance. He then did some trick that makes the estimates of the best predictors a bit more certain that they would otherwise be that I didn't quite understand. There are clear parallel to ensembling and how to pool estimates across learners.

There was also a pretty interesting discussion about Brier scores and what makes for a good forecaster. In particular, I hadn't really thought that it was possible to be a well-calibrated forecaster while also being super cautious (e.g., if the event rate is 50% and you guess 'yes' half of the time); on a calibration curve, this would look like a line just in the middle of the plot. Ideally, you want to be well-calibrated _and decisive_, which are the tails of the calibration plot. 

There was also an interesting discussion about how they used regression to the mean to identify who was actually good at forecasting to those who were simply right by chance. 

The most practice advice can be found in the appendix. To become a better forecaster:

1. Triage. Slope effort. Is it reaosnable to try to predict what you're trying to predict?
2. Break problems into sub-problems. Take a Fermi-like approach.
3. Strike the right balance between the inside and outside view. There's a lot of interesting discussion of this in the book, and overlaps a lot with Kahneman's discussions of base rates. Basically, start with the outside view / base rate, and tweak from there. Maybe another way of putting it is to use Bayes' rule.
4. Strike the right balance between over- and under-reacting to new evidence
5. Look for the clashing causal factors at work in each problem. You should be truth seeking, adn that means understanding both the reasons why a certain outcome could come to pass, while having a really good idea why that outcome might _not_ come to pass. 
6. Strive to distinguish as many degrees of doubt as the problem permits, but no more
7. Strike the right balance between under- and over-confidence
8. Look for the errors behind your mistakes but beware of rearview-mirror hindsight bias. Judge the quality of your decision based on what was knowable at the time and how you pieced that information together. Sometimes great predictions lead to poor outcomes.

My other main takeaway was that people good at forecasting were

- truth-seeking
- curious
- willing to see the problem from a different perspective 