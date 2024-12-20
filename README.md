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
### 1. Central limit theorem (CLT)
#### Definition
The Central Limit Theorem explains that the sample distribution of the sample mean resembles the normal distribution irrespective of the fact that whether the variables themselves are distributed normally or not. <br />

### 2. Shapiro–Wilk test
The Shapiro–Wilk test is **a test of normality**.<br />
 $\displaystyle W={\left(\sum _{i=1}^{n}a_{i}x_{(i)}\right)^{2} \over \sum _{i=1}^{n}(x_{i}-{\overline {x}})^{2}}$ <br />
where
$\displaystyle x_{(i)}$ with parentheses enclosing the subscript index i is the ith order statistic, i.e., the ith-smallest number in the sample (not to be confused with $\displaystyle x_{i}$ ).
$\displaystyle {\overline {x}}=\left(x_{1}+\cdots +x_{n}\right)/n$ is the sample mean.
#### Judgment process:
The larger the p-value of the Shapiro-Wilk test, the more it indicates that the data are close to a normal distribution;
If the p-value is small (e.g., less than 0.05), the original hypothesis is rejected and the data are not considered to be normally distributed.

### 3. Homogeneity of variance test
A method for checking **whether the overall variance is the same for different samples**.
Variance alignment between samples relies heavily on hypothesis testing, and when performing independent samples t-tests and ANOVAs, variance homogeneity can have a greater impact on conclusions than data not satisfying normality.
#### Methods
3.1 F test (the two group should be normal distribution): The F-test constructs a statistic by calculating the ratio of the maximum variance to the minimum variance in the sample and comparing this statistic to one. When the variances of the samples are equal, the F statistic should be close to 1.
$F=\frac{{S_1^2}_{(large)}}{{S_2^2}_{(small)}} $
Bartlett test, Hartley test and Cochran'C test
