# AB Testing Theories

## 1. Central limit theorem (CLT)

### Definition

The Central Limit Theorem explains that the sample distribution of the sample mean resembles the normal distribution irrespective of the fact that whether the variables themselves are distributed normally or not.

## 2. Shapiro–Wilk test

The Shapiro–Wilk test is **a test of normality**.
$$ \displaystyle W={\left(\sum *{i=1}^{n}a*{i}x_{(i)}\right)^{2} \over \sum *{i=1}^{n}(x*{i}-{\overline {x}})^{2}} $$
where x(i) with parentheses enclosing the subscript index i is the ith order statistic, i.e., the ith-smallest number in the sample (not to be confused with xi ). x―=(x1+⋯+xn)/n is the sample mean.

### Judgment process:

The larger the p-value of the Shapiro-Wilk test, the more it indicates that the data are close to a normal distribution; If the p-value is small (e.g., less than 0.05), the original hypothesis is rejected and the data are not considered to be normally distributed.

## 3. Homogeneity of variance test

A method for checking **whether the overall variance is the same for different samples**. Variance alignment between samples relies heavily on hypothesis testing, and when performing independent samples t-tests and ANOVAs, variance homogeneity can have a greater impact on conclusions than data not satisfying normality.

### Methods

3.1 F test (the two group should be normal distribution): The F-test constructs a statistic by calculating the ratio of the maximum variance to the minimum variance in the sample and comparing this statistic to one. When the variances of the samples are equal, the F statistic should be close to 1. $$ F=\frac{{S_1^2}*{(large)}}{{S_2^2}*{(small)}} $$ 

Bartlett test, Hartley test and Cochran'C test

