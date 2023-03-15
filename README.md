# MechaCar_Statistical_Analysis

## Overview
AutosRUs’ newest prototype, the MechaCar, is suffering from production troubles that are blocking the manufacturing team’s progress. AutosRUs’ upper management has called on the data analytics team to review the production data for insights that may help the manufacturing team. The goals of this task are to:

* Perform multiple linear regression analysis to identify which variables in the dataset predict the mpg of MechaCar prototypes.
* Collect summary statistics on the pounds per square inch (PSI) of the suspension coils from the manufacturing lots.
* Run t-tests to determine if the manufacturing lots are statistically different from the mean population.
* Design a statistical study to compare vehicle performance of the MechaCar vehicles against vehicles from other manufacturers. For each statistical analysis, you’ll write a summary interpretation of the findings.

## Linear Regression to Predict MPG
The MechaCar_mpg dataset contains mpg test results for 50 prototype MechaCars. The MechaCar prototypes were produced using multiple design specifications to identify ideal vehicle performance. Multiple metrics, such as vehicle length, vehicle weight, spoiler angle, drivetrain, and ground clearance, were collected for each vehicle. 
### Questions to answer:
* Which variables/coefficients provided a non-random amount of variance to the mpg values in the dataset?
* Is the slope of the linear model considered to be zero? Why or why not?
* Does this linear model predict mpg of MechaCar prototypes effectively? Why or why not?
### Results:
Multiple linear regresssion was performed in order to determine which variables (of those provided in the data) made the most difference in predicting the miles per gallon of the MechCars. The variables used were vehicle length, vehicle weight, spoiler angle, ground clearance and AWD. 

* The most significant variables in our dataset which show a non-random effect on the MPG of the MechaCar are the Vehicle Length and the Ground Clearance. The linear regression model run on these variables against figures for MPG, resulted in p-values of 2.6x10-12 and 5.21x10-8, respectively. The intercept was also statistically significant, indicating that there are likely other factors, not included in our dataset, that have a strong impact on the MPG.
* The slope of the linear model cannot be considered to be zero, since the p-value of 5.35x10-11 near to zero, and thus the null hypothesis should be rejected. This means that the relationship between our variables and the miles per gallon is subject to more than random chance.
•	Residuals are the differences between the prediction and the actual results. The residual values are not small, so although this model does predict the mpg of the MechaCar prototype with some relative effectiveness, a linear model may not be the best fit for this data. However, the r-squared value of 0.7149 indicates that the model is predicts 71%  of the variance in mpg.
<br>
<img src="https://github.com/valchau/MechaCar_Statistical_Analysis/blob/main/summary_p_r_squared_values.PNG" alt="multiple linear regression results" >

## Summary Statistics on Suspension Coils
The MechaCar Suspension_Coil.csv dataset contains the results from multiple production lots. In this dataset, the weight capacities of multiple suspension coils were tested to determine if the manufacturing process is consistent across production lots. 
### Computed results needed to show if the manufacturing process is consistent:
* The suspension coil’s PSI continuous variable across all manufacturing lots.
* The following PSI metrics for each lot: mean, median, variance, and standard deviation.
### Question to answer:
The design specifications for the MechaCar suspension coils dictate that the variance of the suspension coils must not exceed 100 pounds per square inch. Does the current manufacturing data meet this design specification for all manufacturing lots in total and each lot individually? Why or why not?
### Results:
*	While the overall variance is under 100 psi and meets specifications, there is a problem with one of the individual lots. 
*	As shown in the Lot Summary stats, the variance for Lot 3 is well over the acceptable threshold, at 170.28

Here is the overall summary stats:
<br>
<img src="https://github.com/valchau/MechaCar_Statistical_Analysis/blob/main/results_total_summary.PNG" alt="summary stats overall" >
<br>
Here are the summary stats for each of the 3 lots separately:
<br>
<img src="https://github.com/valchau/MechaCar_Statistical_Analysis/blob/main/results_lot_summaryPNG.PNG" alt="summary stats by lot" >

## T-Tests on Suspension Coils
T tests are used to determine if the PSI across all manufacturing lots is statistically different from the population mean of 1,500 pounds per square inch, as well as if each lot is statistically different from the population mean of 1,500 pounds per square inch.
### Questions to answer:
* Determine if the PSI across all manufacturing lots is statistically different from the population mean of 1,500 pounds per square inch.
* Determine if the PSI for each of the 3 manufacturing lots is statistically different from the population mean of 1,500 pounds per square inch.
### Results: 
* The results of the T-test for the suspension coils across all manufacturing lots shows that they are not statistically different from the population mean, and the p-value is not low enough (0.0603) for us to reject the null hypothesis.
<br>
<img src="https://github.com/valchau/MechaCar_Statistical_Analysis/blob/main/t_test_all_lots.PNG" alt="t test for all jobs" >
<br>
* The results of the T-test for the suspension coils for Lot 1 shows that they are not statistically different from the population mean, and the p-value of 1 is not low enough for us to reject the null hypothesis.
<br>
<img src="https://github.com/valchau/MechaCar_Statistical_Analysis/blob/main/t_test_lot1.PNG" alt="t test for lot 1" >
<br>
* The results of the T-test for the suspension coils for Lot 2 shows that they are not statistically different from the population mean, and the p-value is not low enough (0.6072) for us to reject the null hypothesis. 
<br>
<img src="https://github.com/valchau/MechaCar_Statistical_Analysis/blob/main/t_test_lot2.PNG" alt="t test for lot 2" >
<br>
* The results of the T-test for the suspension coils for Lot 3 shows that they are slightly statistically different from the population mean, and the p-value is just low enough (0.0417) for us to reject the null hypothesis. This lot may be need to be discarded, or at least more closely evaluated.
<br>
<img src="https://github.com/valchau/MechaCar_Statistical_Analysis/blob/main/t_test_lot3.PNG" alt="t test for lot 3" >
<br>

## Study Design: MechaCar vs Competition
Here is a statistical study that can quantify how the MechaCar performs against the competition. What metrics would be of interest to a consumer? Suggested metrics are: cost, city or highway fuel efficiency, horse power, maintenance cost, or safety rating.
### Questions to answer: 
* What metric or metrics are you going to test?
* What is the null hypothesis or alternative hypothesis?
* What statistical test would you use to test the hypothesis? And why?
* What data is needed to run the statistical test?



