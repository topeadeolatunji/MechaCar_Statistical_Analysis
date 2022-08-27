# Deliverable 1
## Linear Regression to predict MPG
The MechaCar_mpg.csv file depicts mpg test results for 50 prototype MechaCars. The MechaCar prototypes were produced using multiple design specs to identify prototypes car performance. Multiple metrics, such as car length and weight, spoiler angle and drivetrain were collected for each prototype. Using his knowledge of R, Jeremy designed a linear model that predicts the mpg of MechaCar prototypes using several variables from the MechaCar_mpg.csv data file.

Deliverables:

The MechaCar_mpg.csv file is imported and read into a dataframe through the R console
An RScript is written for a linear regression model to be performed on all six variables
An RScript is written to create the statistical summary of the linear regression model with the intended p-values
There is a summary that addresses all three analysis above (see .R file in github):

Result of linear regression modelling:
<img width="887" alt="image" src="https://user-images.githubusercontent.com/104689265/187011465-125edbf1-3273-42af-9c12-c928c929212b.png">

Statistical summary:
From the above output we can see that:

The car length, and car ground clearance are statistically likely to provide non-random amounts of variance to the model. Therefore, the car length and ground clearance have a significant impact on miles per gallon on the MechaCar prototype. Also, the car weight, spoiler angle, and AWD have p-Values that indicate a random amount of variance with the dataset.

The p-Value for this model, p-Value: 5.35e-11, is much below the significance level of 0.05%. This indicates there is sufficient evidence to reject our null hypothesis, which further indcates that the slope of this linear model is not zero.

This linear model has an r-squared value of 0.7149, which means approximately 71.5% of all mpg predictions will be determined by this model.Concurrently, Jeremy's multiple regression model does predict mpg of MechaCar prototypes effectively.

Removing the less impactful independent variables (car weight, spoiler angle, and AWD), the predictability does decrease, but not drastically: the r-squared value falls from 0.7149 to 0.6825.
