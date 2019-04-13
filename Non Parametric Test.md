* A non parametric test (sometimes called a distribution free test) does not assume anything about the underlying distribution.
* Generally parametric test, which makes assumptions about a population’s parameters (for example, the mean or standard deviation) comes from a normal distribution.
* When the word “non parametric” is used in stats, it doesn’t quite mean that you know nothing about the population. It usually means that you know the population data does not have a normal distribution.
* For example, one assumption for the one way ANOVA is that the data comes from a normal distribution. 
### _If your data isn’t normally distributed, you can’t run an ANOVA, but you can run the nonparametric alternative–the Kruskal-Wallis test_

If at all possible, you should us parametric tests, as they tend to be more accurate. Parametric tests have greater statistical power, which means they are likely to find a true significant effect. Use nonparametric tests only if you have to (i.e. you know that assumptions like normality are being violated). Nonparametric tests can perform well with non-normal continuous data if you have a sufficiently large sample size (generally 15-20 items in each group).

When to use it
Non parametric tests are used when your data isn’t normal. Therefore the key is to figure out if you have normally distributed data. For example, you could look at the distribution of your data. If your data is approximately normal, then you can use parametric statistical tests.
Q. If you don’t have a graph, how do you figure out if your data is normally distributed?
A. Check the skewness and Kurtosis of the distribution using software like Excel (See: Skewness in Excel 2013 and Kurtosis in Excel 2013).
A normal distribution has no skew. Basically, it’s a centered and symmetrical in shape. Kurtosis refers to how much of the data is in the tails and the center. The skewness and kurtosis for a normal distribution is about 1.
