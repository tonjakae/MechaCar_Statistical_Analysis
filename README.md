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

![image](https://user-images.githubusercontent.com/87340105/156869935-d2c263f5-bb5d-4dfb-9b9d-4f44da7a3280.png)

![image](https://user-images.githubusercontent.com/87340105/156869975-37b2e515-dbbe-49b8-afe9-2880fc8db322.png)

![image](https://user-images.githubusercontent.com/87340105/156869982-0fa09d70-c36f-41e6-b402-5097638ae737.png)

### 1.) The design specifications for the MechaCar suspension coils dictate that the variance of the suspension coils must not exceed 100 pounds per square inch. Does the current manufacturing data meet this design specification for all manufacturing lots in total and each lot individually? Why or why not?



##### -
## T-Test on Suspension Coils



## Design a Study Comparing the MechaCar to the Competition
