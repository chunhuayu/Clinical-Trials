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
