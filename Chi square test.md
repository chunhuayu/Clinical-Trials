# The Chi Square statistic
* commonly used for testing relationships between categorical variables.  
* The null hypothesis of the Chi-Square test is that no relationship exists on the categorical variables in the population; 
* They are independent.  
### An example research question that could be answered using a Chi-Square analysis would be:
* Is there a significant relationship between voter intent and political party membership?
# How does the Chi-Square statistic work?
* The Chi-Square statistic is most commonly used to evaluate Tests of Independence when using a crosstabulation (also known as a bivariate table).  
* Crosstabulation presents the distributions of two categorical variables simultaneously, with the intersections of the categories of the variables appearing in the cells of the table.  
* The Test of Independence assesses whether an association exists between the two variables by comparing the observed pattern of responses in the cells to the pattern that would be expected if the variables were truly independent of each other.  
* Calculating the Chi-Square statistic and comparing it against a critical value from the Chi-Square distribution allows the researcher to assess whether the observed cell counts are significantly different from the expected cell counts.
![Mou icon](https://www.statisticssolutions.com/wp-content/uploads/2011/05/ch1.png)
* where fo = the observed frequency (the observed counts in the cells)
* fe = the expected frequency if NO relationship existed between the variables
* As depicted in the formula, the Chi-Square statistic is based on the difference between what is actually observed in the data and what would be expected if there was truly no relationship between the variables.
* sum((fo-fe)^2/fe)
### What are special concerns with regard to the Chi-Square statistic?
* There are a number of important considerations when using the Chi-Square statistic to evaluate a crosstabulation.  
* Because of how the Chi-Square value is calculated, it is extremely sensitive to sample size – when the sample size is too large (~500), * almost any small difference will appear statistically significant.  
* It is also sensitive to the distribution within the cells, and some of Statistical software gives a warning message if cells have fewer than 5 cases. 
* This can be addressed by always using categorical variables with a limited number of categories (e.g., by combining categories if necessary to produce a smaller table).
### an example
> k variable has three levels . w variable has two exclusive levels. there is an association between k and w.

|table|level 1 | level 2 | level 3|
|:---:|:------:|:-------:|:-----:|
|forvor|892|1165|954|
|oppose|185|149|66|

### chi square test table
|Statistic| DF| Value| Prob |
|:-------:|:-----:|:-----:|:-----:|
|Chi-Square| 2| 58.3229| <.0001| 
|Likelihood Ratio Chi-Square| 2 |59.5927 |<.0001 |
| Mantel-Haenszel Chi-Square |1| 58.1227 |<.0001 |
|Phi Coefficient|  | 0.1308|   |
|Contingency Coefficient | | 0.1297||   
|Cramer's V|  | 0.1308||   
### conclusion 
The p-value(<0.0001) indicates that these variables are not independent of each other and that there is a statistically significant relationship between the categorical variables.

### The following is SAS code for this example.
      data chi2;
      do k= 1 to 2;
      do w= 1 to 3;
      input x @@;
      output;
      end;
      end;
      cards;
      892 1165 954 185 149 66
      ;
      proc freq data=chi2;
      tables k* w/ chisq;
      weight x;
      run;
### The following is R code for this example.
      kw=matrix(c(892,1165,954,185,149,66),ncol = 3)
      chisq.test(kw)
###### The output of R
      Pearson's Chi-squared test
      data:  kw
      X-squared = 503.7, df = 2, p-value < 2.2e-16
