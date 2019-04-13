* A non parametric test (sometimes called a distribution free test) does not assume anything about the underlying distribution.
* Generally parametric test, which makes assumptions about a population’s parameters (for example, the mean or standard deviation) comes from a normal distribution.
* When the word “non parametric” is used in stats, it doesn’t quite mean that you know nothing about the population. It usually means that you know the population data does not have a normal distribution.
* For example, one assumption for the one way ANOVA is that the data comes from a normal distribution. 
### _If your data isn’t normally distributed, you can’t run an ANOVA, but you can run the nonparametric alternative–the Kruskal-Wallis test_

* If at all possible, you should do parametric tests, as they tend to be more accurate. Parametric tests have greater statistical power, which means they are likely to find a true significant effect. 
* Use nonparametric tests only if you have to (i.e. you know that assumptions like normality are being violated).
* Nonparametric tests can perform well with non-normal continuous data if you have a sufficiently large sample size (generally 15-20 items in each group).

### When to use it
* Non parametric tests are used when your data isn’t normal. Therefore the key is to figure out if you have normally distributed data. 
* For example, you could look at the distribution of your data. If your data is approximately normal, then you can use parametric statistical tests.
* Q. If you don’t have a graph, how do you figure out if your data is normally distributed?
* A. Check the __skewness and Kurtosis of the distribution__ using software like Excel.
* A normal distribution has no skew. Basically, it’s a centered and symmetrical in shape. Kurtosis refers to how much of the data is in the tails and the center. 
* The skewness and kurtosis for a normal distribution is about 1.

### Data Types
* Does your data allow for a parametric test, or do you have to use a non parametric test like chi-square? The rule of thumb is:
> For nominal scales or ordinal scales, use non parametric statistics.
> For interval scales or ratio scales use parametric statistics.

### Other reasons to run nonparametric tests
* One or more assumptions of a parametric test have been violated.
* Your sample size is too small to run a parametric test.
* Your data has outliers that cannot be removed.
* You want to test for the median rather than the mean (you might want to do this if you have a very skewed distribution).

# Types of Nonparametric Tests
* When the word “parametric” is used in stats, it usually means tests like ANOVA or a t test. Those tests both assume that the population data has a normal distribution. 
* Non parametric do not assume that the data is normally distributed. 
* The only non parametric test you are likely to come across in elementary stats is the chi-square test. 
#### However, there are several others 
* __For example: the Kruskal Willis test is the non parametric alternative to the One way ANOVA and the Mann Whitney is the non parametric alternative to the two sample t test.__

# The main nonparamteric tests are:
* 1-sample sign test. Use this test to estimate the median of a population and compare it to a reference value or target value.
* 1-sample Wilcoxon signed rank test. With this test, you also estimate the population median and compare it to a reference/target value. However, the test assumes your data comes from a symmetric distribution (like the Cauchy distribution or uniform distribution).
* Friedman test. This test is used to test for differences between groups with ordinal dependent variables. It can also be used for continuous data if the one-way ANOVA with repeated measures is inappropriate (i.e. some assumption has been violated).
* Goodman Kruska’s Gamma: a test of association for ranked variables.
* Kruskal-Wallis test. Use this test instead of a one-way ANOVA to find out if two or more medians are different. Ranks of the data points are used for the calculations, rather than the data points themselves.
* The Mann-Kendall Trend Test looks for trends in time-series data.
* Mann-Whitney test. Use this test to compare differences between two independent groups when dependent variables are either ordinal or continuous.
Mood’s Median test. Use this test instead of the sign test when you have two independent samples.
Spearman Rank Correlation.Use when you want to find a correlation between two sets of data.
