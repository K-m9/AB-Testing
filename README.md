# ABTest
## Definition
An online control experiment, aiming to inferencing the casual relationship and quantified effect of the improvement, with the use of Hypothesis testing.<br />
Control group (A): nothing changed; Treatment group (B): change the function or strategy.
### Characteristics
- Homogeneity: the sample proportion of A and B is consistent;
- Simultaneity: the same time to do the experiment of group A and B;
- Randomness: Different users are randomly divided into different groups;
## Process of  ABTest
### before the test
1. finding the improvement point of the product.
2. make sure how to improve the product: changing the function, changing the strategy...
3. decide the core index (CVR, ....) and auxiliary index.
### In the test
1. Choosing the experimental population and the population size.
2. Set the experiment parameter.
3. AA TEST.
### After the test
1. data analysis: Hypothesis test
2. Make a decision of whether to accept the change.

## Theories
### Central limit theorem (CLT)
#### Definition
The Central Limit Theorem explains that the sample distribution of the sample mean resembles the normal distribution irrespective of the fact that whether the variables themselves are distributed normally or not. <br />
Let us assume we have a random variable X. Let σ be its standard deviation and μ is the mean of the random variable. Now as per the Central Limit Theorem, the sample mean \overline{X}  will approximate to the normal distribution which is given as \overline{X} ⁓ N(μ, σ/√n). The Z-Score of the random variable \overline{X}  is given as Z = \dfrac{\overline x – \mu}{\frac{\sigma}{\sqrt n}} . Here \overline x  is the mean of \overline X . The image of the formula is attached below.
