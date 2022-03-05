# MechaCar Statistical Analysis

## Overview
AutosRUs’ newest prototype, the MechaCar, is suffering from production troubles that are blocking the manufacturing team’s progress. AutosRUs’ upper management has called on Jeremy and the data analytics team to review the production data for insights that may help the manufacturing team.

## Resources
* R 4.1.2 
* MechaCar_mpg.csv
* Suspension_Coil.csv

# Summary: Linear Regression to Predict MPG

![image](https://user-images.githubusercontent.com/87340105/156869849-798c005f-7d0d-4690-bf48-9be51f46375f.png)

![image](https://user-images.githubusercontent.com/87340105/156869703-00935023-0274-471c-b39c-494411745626.png)

### 1.) Which variables/coefficients provided a non-random amount of variance to the mpg values in the dataset? 
The vehicle length, and vehicle ground clearance are statistically likely to provide non-random amounts of variance to the model. That is to say, the vehicle length and vehicle ground clearance have a significant impact on miles per gallon on the MechaCar prototype. Conversely, the vehicle weight, spoiler angle, and All Wheel Drive (AWD) have p-Values that indicate a random amount of variance with the dataset.

### 2.) Is the slope of the linear model considered to be zero? Why or why not? 
The p-Value for this model, is 5.35e-11, which is smaller than the assumed significance level of 0.05%. This indicates that the slope of this linear model is not zero.

### 3.) Does this linear model predict mpg of MechaCar prototypes effectively? Why or why not? 
This model has an r-squared value of 0.7149, which means that approximately 71% of all mpg predictions will be determined by this model. This mmodel does predict mpg of MechaCar prototypes effectively.

###### -
# Summary: Statistics on Suspension Coils

Write an RScript that creates a total_summary dataframe using the summarize() function to get the mean, median, variance, and standard deviation of the suspension coil’s PSI column.

#### Total Summary
![image](https://user-images.githubusercontent.com/87340105/156870721-c4a67ce1-9941-413c-8dc1-8840b82f1109.png)

Write an RScript that creates a lot_summary dataframe using the group_by() and the summarize() functions to group each manufacturing lot by the mean, median, variance, and standard deviation of the suspension coil’s PSI column.

#### Lot Summary
![image](https://user-images.githubusercontent.com/87340105/156870729-95124fae-28c7-4645-ad4e-c36a705c11ce.png)


### 1.) The design specifications for the MechaCar suspension coils dictate that the variance of the suspension coils must not exceed 100 pounds per square inch. Does the current manufacturing data meet this design specification for all manufacturing lots in total and each lot individually? Why or why not?
When looking at the overall data we can see that the design specification for all lots combined does meet the variance requirements of the PSI.  When looking at each lot individually however, Lot 3 is not meeting that specification as the variance is 170.29 and the standard deviation is 13.05. Lots 1 and 2 continue to meet the required specifications individually.


##### -
## Summary: T-Test on Suspension Coils

Write an RScript using the t.test() function to determine if the PSI across all manufacturing lots is statistically different from the population mean of 1,500 pounds per square inch.

#### 1.) The t-test for the entire population provides a p-value of 0.06. There is not sufficient evidence to reject the null hypothesis.

![image](https://user-images.githubusercontent.com/87340105/156871300-4e4784dc-59fe-47b6-90b7-5c4c0c924032.png)

Write three more RScripts in your MechaCarChallenge.RScript using the t.test() function and its subset() argument to determine if the PSI for each manufacturing lot is statistically different from the population mean of 1,500 pounds per square inch.

#### 2.) The t-test for Lot 1 shows a p-value of 1, which means there is not sufficient evidence to reject the null hypothesis.

![image](https://user-images.githubusercontent.com/87340105/156871229-602179db-a41b-4161-bbd1-8e7cbcc79f12.png)

#### 3.) The t-test for Lot 2 shows a p-value of .61, which means there is not sufficient evidence to reject the null hypothesis.

![image](https://user-images.githubusercontent.com/87340105/156871257-3e73e458-23f1-4d46-a8cf-ab2cd4ff8e6d.png)

#### 4.) The t-test for Lot 3 shows a p-value of 0.042, which means there is sufficient statistical evidence to reject the null hypothesis. Lot 3's mean PSI is statistically different from the whole populations's mean PSI.

![image](https://user-images.githubusercontent.com/87340105/156871268-e44e573c-0961-4442-86e4-ea012f13b0a3.png)
