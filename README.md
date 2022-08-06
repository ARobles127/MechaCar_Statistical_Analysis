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



## Summary Statistics on Suspension Coils

The second part of the project is to analyze the Suspension_Coil data set that  contains the results from multiple production lots. In this dataset, the weight capacities of multiple suspension coils were tested to determine if the manufacturing process is consistent across production lots. To accomplish our tasks we will create a summary statistics table to show the suspension coil’s PSI continuous variable across all manufacturing lots, and the PSI metrics for each lot: mean, median, variance, and standard deviation. Refer to the two tables below to see the results.


![total_summary.png]()


![lot_summary.png]()

The design specifications for the MechaCar suspension coils dictate that the variance of the suspension coils must not exceed 100 pounds per square inch. Does the current manufacturing data meet this design specification for all manufacturing lots in total and each lot individually? Why or why not?  Looking at the results from our tables above, we can conclude that the variance from our lot_summary value is 62.29356, which is within  the specified value and does not exceed the 100 pounds per square inch variance. However, when we look at each single lot, we can see each value and conclude  that Lots 1 and 2 are within this value, but Lot 3  does not meet the requirement.   



## T-Tests on Suspension Coils

For this part of the project we are going to apply T-Test on our Suspension Coils data set to determine if all manufacturing lots and each lot individually are statistically different from the population mean of 1,500 pounds per square inch.

The following image provides the results from the T-test applied to the suspension coil data, from which we conclude that the mean value in this dataset, 1489.7,  is slightly different from the population mean of 1,500 pounds per square inch. The p-value is equal to 0.06028 which is above the ideal value (0.05), in consequence, there is not enough evidence to reject the null hypothesis.  


![t_test1.png]()



Subsequently, we analyzed each of the manufacturing lots by applying a T-test to determine if the PSI for each manufacturing lot is statistically different from the population mean of 1,500 pounds per square inch. From the results we determined that there is not  sufficient evidence to reject the null hypothesis, since the p-value on all three tests is above  the common 0.05 percent value. The other metric to be considered is the  mean. The results show that the mean variance on all three tests is minimal to the population mean of 1,500 pounds per square inch.


![ttest_lot1.png]()


![ttest_lot2.png]()


![ttest_lot3.png]()



