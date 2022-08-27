# Deliverable 1
## Linear Regression to predict MPG
The MechaCar_mpg.csv file depicts mpg test results for 50 prototype MechaCars. The MechaCar prototypes were produced using multiple design specifications to identify ideal vehicle performance. Multiple metrics, such as vehicle length, vehicle weight, spoiler angle, drivetrain, and ground clearance, were collected for each vehicle. Using your knowledge of R, you’ll design a linear model that predicts the mpg of MechaCar prototypes using several variables from the MechaCar_mpg.csv file.

Deliverables:

The MechaCar_mpg.csv file is imported and read into a dataframe through the R console
An RScript is written for a linear regression model to be performed on all six variables
An RScript is written to create the statistical summary of the linear regression model with the intended p-values
There is a summary that addresses all three questions:

Result of linear regression modelling:
<img width="887" alt="image" src="https://user-images.githubusercontent.com/104689265/187011465-125edbf1-3273-42af-9c12-c928c929212b.png">

Statistical summary:
From the above output we can see that:

The vehicle length, and vehicle ground clearance are statistically likely to provide non-random amounts of variance to the model. That is to say, the vehicle length and vehicle ground clearance have a significant impact on miles per gallon on the MechaCar prototype. Conversely, the vehicle weight, spoiler angle, and All Wheel Drive (AWD) have p-Values that indicate a random amount of variance with the dataset.

The p-Value for this model, p-Value: 5.35e-11, is much smaller than the assumed significance level of 0.05%. This indicates there is sufficient evidence to reject our null hypothesis, which further indcates that the slope of this linear model is not zero.

This linear model has an r-squared value of 0.7149, which means that approximately 71% of all mpg predictions will be determined by this model. Relatively speaking, his multiple regression model does predict mpg of MechaCar prototypes effectively.

If we remove the less impactful independent variables (vehicle weight, spoiler angle, and All Wheel Drive), the predictability does decrease, but not drastically: the r-squared value falls from 0.7149 to 0.674.
