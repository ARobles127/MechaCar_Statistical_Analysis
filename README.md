# MechaCar_Statistical_Analysis
RStudio

In this project we are going to apply statistical tests to help AutosRUs make informed decisions based on data analysis using R, a programming language that has a variety of uses in data science. R has solidified itself in academia and industry as one of the go-to programming languages for statistical modeling and hypothesis testing. 



## Linear Regression to Predict MPG

For the first part of the project we are going to analyze a dataset that contains mpg test results for 50 prototype MechaCars. The MechaCar prototypes were produced using multiple design specifications to identify ideal vehicle performance. To accomplish our task we will  design a linear model that predicts the mpg of MechaCar prototypes using several variables from the data file. 


![LR_Formula.npg]() 

- Which variables/coefficients provided a non-random amount of variance to the mpg values in the dataset?
According to our results the Vehicle_weight, spoiler_angle , AWD  provided a non-random amount of variance, meaning that these variables have a significant impact on the mpg value in the dataset.

- Is the slope of the linear model considered to be zero? Why or why not?
Yes,  the p-value: 5.35e-11, which is much smaller than the expected  0.05% value. Therefore, we can state that there is sufficient evidence to reject the null hypothesis, which means that the slope of our linear model is not zero.

- Does this linear model predict mpg of MechaCar prototypes effectively? Why or why not?
Yes, in accordance with the results, the Multiple R-squared:  0.7149 value represents 71% of the variability of the dependent variable (mpg), which means that in a simple linear regression model, the higher the correlation is between two variables, the more that one variable can explain/predict the value of the other.
