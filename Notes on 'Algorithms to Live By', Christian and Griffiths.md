# Notes on 'Algorithms to Live By', Christian and Griffiths

## optimal stopping

- **37% rule**: If you have no information about the distribution of, say, apartments, how many do you look at before making a decision? If you have 10 days, take the first 4 days (~37% of 10) just to sample apartments, then choose based on the information you've gained during those 4 days. Unfortunately, you'll only get the best apartment 37% of the time with this approach.
- If we know how good the apartments are (e.g. this is in the 95th percentile of all apartments), then use the **threshold rule**. The exact threshold depends on the number of apartments or applicants in the pool. For >=10 applicants, only accept applicants >= the 90th percentile.

## explore / exploit

- "People tend to focus on decisions in isolation, to focus on finding each time the outcome with the highest expected value. But decisions are almost never isolated, and expected value isn't the end of the story." p. 34
- When deciding whether to stay somewhere that gives you some pay-off of switch to someplace else, **win-stay lose-shift** performs better than chance.
- The __Gittins index__ is a really interesting idea but the book explains it poorly.
- To minimize regret, use the __upper confidence bound__  algorithm. Choose the option that has the highest upper confidence interval. For example, a restaurants that you've sampled a couple times will have a wide confidence interval because you're still pretty unsure of how good it is; if you've eaten at a restaurant a lot, the confidence bounds are sharper.

## sorting

- __bubble sort__: make passes across an array, switching consecutive items when they are not ordered. Very slow.
- __insertion sort__: Build the array iteratively, by placing the first thing in a new array. Put the second thing either to the right or left or the first thing. Sweep through the new array left to right to determine where the third thing goes, and so on. Also very slow.
- __Mergesort__: If you have two sorted arrays, you just have to compare the top elements of each of the sorted arrays to add to the new array. Easily parallelized. Fast.
- __Bucket sort:__ Sort things into rough 'buckets' or categorizes. Fast.

## caching

- __First-in, first-out__: when full, evict whatever's been in your cache (or closest) the longest.
- __least recently used:__ evict the thing that gone longest untouched. This is generally the best algorithm.

## scheduling

- __earliest due date__: order things to do by due date, then work on whatever due date is closest. Minimizes maximal lateness.
- __shortest processing time:__ do the fastest task first. Maximizes the number of things you get done. 
- The optimal strategy is usually to enumerate the weight (how good you'll feel if you get the thing done) and the amount of time it will take. Divide the latter by the former, sort, and do the 'densest' thing first.

## baye's rule

- **Laplace's Law:** Used for estimating probabilities that some binary outcome happens based on prior experience. Let w = number of times the thing has happened in the past. Let n = total number of opportunities it could have happened. The best guess for the probability is then (w + 1) / (n + 2).
- __Copernican Principle:__ When you have no idea how long something will exist / last, the best guess is twice as long as it's already lasted.
- __Multiplicative rule:__ Given an uninformative prior, to estimate some quantity multiply the number observed by some constant (in the case of the Copernican Principle, that constant is two). 
- __average rule:__ when prior is normal, guess the mean.
- __additive rule:__ when the prior is Erlang, guess the current amount + some constant. 

## overfitting

- __cross validation:__ seeing how well a model generalizes to new data
- __regularization:__ penalize complexity
- __early stopping:__ stop optimization before things have gotten too complex

## relaxation

- __constraint relaxation:__ If a problem is too hard, relax one of the constraints.

## game theory

- interesting idea: __Vickrey auction__. Sealed auction where everyone writes down a single number they want to pay for something. The winner is the person who writes down the highest bid, but they pay the second-highest price. Best option is honesty. 
