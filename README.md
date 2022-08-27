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

# Deliverable 2
## Summary Statistics on Suspension Coils
The MechaCar Suspension_Coil.csv data file has the results from multiple production lots. In this dataset, the weight capacities of multiple suspension coils were tested to determine if the manufacturing process is consistent across production lots. Using your knowledge of R, Jeremy created a summary statistics table to show:

The suspension coil’s PSI continuous variable across all manufacturing lots
The following PSI metrics for each lot: mean, median, variance, and standard deviation.

The Suspension Coil dataset provided for the MechaCar contains the results of testing the weight capacities of multiple suspension coils from multiple production lots to determine consistency.

First looking at all manufacturing lots:

<img width="588" alt="image" src="https://user-images.githubusercontent.com/104689265/187015384-8a964bc2-8560-4b10-a5cc-61e0f26adeff.png">

Diving a little deeper into each of the 3 lots:

<img width="908" alt="image" src="https://user-images.githubusercontent.com/104689265/187015429-19cd1b60-38f5-47cd-8263-d2f9c64b126e.png">

With the understanding that the design specs for the MechaCar suspension coils mandate that the variance of the suspension coils cannot exceed 100 pounds per square inch (PSI) .

When looking at the entire population of the production lot, the variance of the coils is 62.29 PSI, which is well within the 100 PSI variance requirement.

Similarly, but significantly more consistent, Lot 1 and Lot 2 are well within the 100 PSI variance requirement; with variances of 0.98 and 7.47 respectively. However, it is Lot 3 that is showing a much larger variance in performance and consistency, with a variance of 170.29. It is Lot 3 that is disproportionately causing the variance at the full lot level.

# Deliverable 3

## t-Tests on Suspension Coils

From here we can see the true mean of the sample is 1498.78, which we also saw in the summary statistics above. With a p-Value of 0.06, which is higher than the common significance level of 0.05, there is NOT enough evidence to support rejecting the null hypothesis. That is to say, the mean of all three of these manufacturing lots is statistically similar to the presumed population mean of 1500.

Next looking at each individual lots:

Lot 1 sample actually has the true sample mean of 1500, again as we saw in the summary statistics above. With a p-Value of 1, clearly we cannot reject (i.e. accept) the null hypothesis that there is no statistical difference between the observed sample mean and the presumed population mean (1500).
Lot 2 has essentially the same outcome with a sample mean of 1500.02, a p-Value of 0.61; the null hypothesis cannot be rejected, and the sample mean and the population mean of 1500 are statistically similar.
However, Lot 3, not surprisingly is a different scenario. Here the sample mean is 1496.14 and the p-Value is 0.04, which is lower than the common significance level of 0.05. All indicating to reject the null hypothesis that this sample mean and the presumed population mean are not statistically different.

# Deliverable 4

## Study Design: MechaCar vs Competition

Metrics

Collecting data for comparable models across all major manufacturers for past 3 years for the following metrics:

Safety Feature Rating: Independent Variable
Current Price (Selling): Dependent Variable
Drive Package : Independent Variable
Engine (Electric, Hybrid, Gasoline / Conventional): Independent Variable
Resale Value: Independent Variable
Average Annual Cost of ownership (Maintenance): Independent Variable
MPG (Gasoline Efficiency): Independent Variable
Hypothesis: Null and Alternative

After determining which factors are key for the MechaCar's genre:

Null Hypothesis (Ho): MechaCar is priced correctly based on its performance of key factors for its genre.
Alternative Hypothesis (Ha): MechaCar is NOT priced correctly based on performance of key factors for its genre.
Statistical Tests

A multiple linear regression would be used to determine the factors that have the highest correlation/predictability with the list selling price (dependent variable); which combination has the greatest impact on price (it may be all of them!)


