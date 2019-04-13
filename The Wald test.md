# The Wald test 
* (also called the Wald Chi-Squared Test) is a way to find out if explanatory variables in a model are significant.
* The test can be used for a multitude of different models including those with binary variables or continuous variables.
## The Wald test is usually talked about in terms of chi-squared
* Because the sampling distribution (as n approaches infinity) is usually known. 
* This variant of the test is sometimes called the Wald Chi-Squared Test to differentiate it from the Wald Log-Linear Chi-Square Test, which is a non-parametric variant based on the log odds ratios.


# Significant 
* Means that they add something to the model; 

# Insignificant
* Variables that add nothing can be deleted without affecting the model in any meaningful way. 

# The null hypothesis for the test is: 
* some parameter = some value. 
* __For example__:
you might be studying if weight is affected by eating junk food twice a week. “Weight” would be your parameter. The value could be zero (indicating that you don’t think weight is affected by eating junk food). If the null hypothesis is rejected, it suggests that the variables in question can be removed without much harm to the model fit. 
If the Wald test shows that the parameters for certain explanatory variables are zero, you can remove the variables from 
the model. If the test shows the parameters are not zero, you should include the variables in the model. 

