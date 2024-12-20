# AB Testing Theories

## 1. Central limit theorem (CLT)

### Definition

The Central Limit Theorem explains that the sample distribution of the sample mean resembles the normal distribution irrespective of the fact that whether the variables themselves are distributed normally or not.

## 2. Normality test

https://courses.washington.edu/psy524a/pdf/Normality_Tests.pdf



### 2.1 Kolmogorov-Smirnov test

https://www.cnblogs.com/jiangkejie/p/11572205.html

https://www.geeksforgeeks.org/kolmogorov-smirnov-test-ks-test/

Disadvantages: only applies to **continuous distributions**; sensitive in the middle of the distribution, not sensitive enough at the ends; the biggest limitation is that the entire distribution needs to be completely determined, and if parameters such as position, shape, etc., are estimated from the data, the decision intervals are no longer valid, and therefore these parameters can generally only be obtained by simulation.

### 2.2 Shapiro–Wilk test

The Shapiro–Wilk test is **a test of normality**.
$$
\displaystyle W={\left(\sum *{i=1}^{n}a*{i}x_{(i)}\right)^{2} \over \sum *{i=1}^{n}(x*{i}-{\overline {x}})^{2}}
$$

where x(i) with parentheses enclosing the subscript index i is the ith order statistic, i.e., the ith-smallest number in the sample (not to be confused with xi ). $\bar{x} =(x1+⋯+xn)/n$ is the sample mean.

#### Judgment process:

The larger the p-value of the Shapiro-Wilk test, the more it indicates that the data are close to a normal distribution; If the p-value is small (e.g., less than 0.05), the original hypothesis is rejected and the data are not considered to be normally distributed.

## 3. Homogeneity of variance test

A method for checking **whether the overall variance is the same for different samples**. Variance alignment between samples relies heavily on hypothesis testing, and when performing independent samples t-tests and ANOVAs, variance homogeneity can have a greater impact on conclusions than data not satisfying normality.

### Methods

#### 3.1 F test **(the two group should be normal distribution)**

 The F-test constructs a statistic by calculating the ratio of the maximum variance to the minimum variance in the sample and comparing this statistic to one. When the variances of the samples are equal, the F statistic should be close to 1. 
$$
F=\frac{{S_1^2}*{(large)}}{{S_2^2}*{(small)}}
$$


#### 3.2 Bartlett test **(the two group should be normal distribution) **



#### 3.3 Hartley test **(the two group should be normal distribution) **

The test involves computing the of the largest group variance, max(sj2) to the smallest group variance, min(sj2). The resulting ratio, Fmax, is then compared to a critical value from a table of the of Fmax. If the computed ratio is less than the critical value, the groups are assumed to have similar or equal variances.

Hartley's test assumes that data for each group are normally distributed and that **each group has an equal number of members**. 

#### 3.4 Cochran'C test (the two group should be normal distribution)

#### 3.5 Levene test (non-normal distribution)

The basic idea of Levene's method is to use the F-value test to determine the differences between groups after centering the values of the variables in each group.
$$
W = \frac{N-k}{k-1}\times\frac{\sum_{i = 1}^{k}n_i(D_i - \overline{D})^2}{\sum_{i =1}^k\sum_{j = 1}^{n_i}(d_{ij} - D_i)^2}
$$


## Two-sample hypothesis testing

https://www.me.psu.edu/cimbala/me345/Lectures/Two_Samples_Hypothesis_Testing.pdf

### Mann-Whitney U Test (**two sample Wilcoxon test**)

https://stats.libretexts.org/Bookshelves/Applied_Statistics/Learning_Statistics_with_R_-_A_tutorial_for_Psychology_Students_and_other_Beginners_(Navarro)/13%3A_Comparing_Two_Means/13.10%3A__Testing_Non-normal_Data_with_Wilcoxon_Tests

the Shapiro-Wilk test made it very clear that the normality assumption is violated. This is the situation where you want to use Wilcoxon tests.

A **Mann-Whitney U test** (sometimes called the Wilcoxon rank-sum test) is used to compare the differences between two independent samples when the sample distributions are not normally distributed and the sample sizes are small (n <30).

It is considered to be the **nonparametric** equivalent to the two-sample independent t-test.
