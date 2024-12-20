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

### Shapiro–Wilk test
The Shapiro–Wilk test is a test of normality.
<math xmlns="http://www.w3.org/1998/Math/MathML" display="block"><mstyle displaystyle="true" scriptlevel="0"><mi>W</mi><mo>=</mo><mrow><mfrac><msup><mrow data-mjx-texclass="INNER"><mo data-mjx-texclass="OPEN">(</mo><munderover><mo data-mjx-texclass="OP">∑</mo><mrow><mi>i</mi><mo>=</mo><mn>1</mn></mrow><mrow><mi>n</mi></mrow></munderover><msub><mi>a</mi><mrow><mi>i</mi></mrow></msub><msub><mi>x</mi><mrow><mo stretchy="false">(</mo><mi>i</mi><mo stretchy="false">)</mo></mrow></msub><mo data-mjx-texclass="CLOSE">)</mo></mrow><mrow><mn>2</mn></mrow></msup><mrow><munderover><mo data-mjx-texclass="OP">∑</mo><mrow><mi>i</mi><mo>=</mo><mn>1</mn></mrow><mrow><mi>n</mi></mrow></munderover><mo stretchy="false">(</mo><msub><mi>x</mi><mrow><mi>i</mi></mrow></msub><mo>−</mo><mrow><mover><mi>x</mi><mo accent="false">¯</mo></mover></mrow><msup><mo stretchy="false">)</mo><mrow><mn>2</mn></mrow></msup></mrow></mfrac></mrow></mstyle></math>
where
$\displaystyle x_{(i)}$ with parentheses enclosing the subscript index i is the ith order statistic, i.e., the ith-smallest number in the sample (not to be confused with $\displaystyle x_{i}$ ).
$\displaystyle {\overline {x}}=\left(x_{1}+\cdots +x_{n}\right)/n$ is the sample mean.
#### Judgment process:
The larger the p-value of the Shapiro-Wilk test, the more it indicates that the data are close to a normal distribution;
If the p-value is small (e.g., less than 0.05), the original hypothesis is rejected and the data are not considered to be normally distributed.
