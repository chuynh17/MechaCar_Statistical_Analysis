# MechaCar_Statistical_Analysis


## Linear Regression to Predict MPG

![Screen Shot 2021-06-26 at 22 56 11](https://user-images.githubusercontent.com/79731109/123551282-b7fdc700-d736-11eb-9365-b7d061338e93.png)


#### Which variables/coefficients provided a non-random amount of variance to the mpg values in the dataset?

The vehicle length, and vehicle ground clearance are statistically likely to provide non-random amounts of variance to the model. That is to say, the vehicle length and vehicle ground clearance have a significant impact on miles per gallon on the MechaCar prototype. Conversely, the vehicle weight, spoiler angle, and All Wheel Drive (AWD) have p-Values that indicate a random amount of variance with the dataset.

#### Is the slope of the linear model considered to be zero? Why or why not?

The p-Value for this model, p-Value: 5.35e-11, is much smaller than the assumed significance level of 0.05%. This indicates there is sufficient evidence to reject our null hypothesis, which further indcates that the slope of this linear model is not zero.
#### Does this linear model predict mpg of MechaCar prototypes effectively? Why or why not?

This linear model has an r-squared value of 0.7149, which means that approximately 71% of all mpg predictions will be determined by this model. Relatively speaking, his multiple regression model does predict mpg of MechaCar prototypes effectively.

## Summary Statistics on Suspension Coils

#### The design specifications for the MechaCar suspension coils dictate that the variance of the suspension coils must not exceed 100 pounds per square inch. 

![Screen Shot 2021-06-27 at 11 08 32](https://user-images.githubusercontent.com/79731109/123551593-1f684680-d738-11eb-9ce9-604def5920c0.png)

#### Does the current manufacturing data meet this design specification for all manufacturing lots in total and each lot individually? Why or why not?

![Screen Shot 2021-06-27 at 11 08 15](https://user-images.githubusercontent.com/79731109/123551603-25f6be00-d738-11eb-9946-2fc102279609.png)

When looking at the entire population of the production lot, the variance of the coils is 62.29 PSI, which is well within the 100 PSI variance requirement.

Similarly, but significantly more consistent, Lot 1 and Lot 2 are well within the 100 PSI variance requirement; with variances of 0.98 and 7.47 respectively. However, it is Lot 3 that is showing much larger variance in performance and consistency, with a variance of 170.29. It is Lot 3 that is disproportionately causing the variance at the full lot level.


## T-Tests on Suspension Coils

### Summarized T-Test
![Screen Shot 2021-06-26 at 23 09 15](https://user-images.githubusercontent.com/79731109/123554503-ef27a480-d745-11eb-964d-d3d14d9006a1.png)

From here we can see the true mean of the sample is 1498.78, which we also saw in the summary statistics above. With a p-Value of 0.06, which is higher than the common significance level of 0.05, there is NOT enough evidence to support rejecting the null hypothesis. That is to say, the mean of all three of these manufacturing lots is statistically similar to the presumed population mean of 1500.

### T-Test on Lot 1
![Screen Shot 2021-06-26 at 23 09 30](https://user-images.githubusercontent.com/79731109/123554506-f189fe80-d745-11eb-90c7-d49e523ef520.png)

Lot 1 sample actually has the true sample mean of 1500, again as we saw in the summary statistics above. With a p-Value of 1, clearly we cannot reject (i.e. accept) the null hypothesis that there is no statistical difference between the observed sample mean and the presumed population mean (1500).

### T-Test on Lot 2
![Screen Shot 2021-06-26 at 23 09 30](https://user-images.githubusercontent.com/79731109/123554511-f5b61c00-d745-11eb-9099-60a77e4ba7ba.png)

Lot 2 has essentially the same outcome with a sample mean of 1500.02, a p-Value of 0.61; the null hypothesis cannot be rejected, and the sample mean and the population mean of 1500 are statistically similar.

### T-Test on Lot 3
![Screen Shot 2021-06-26 at 23 09 49](https://user-images.githubusercontent.com/79731109/123554518-fa7ad000-d745-11eb-9853-a3c5f019263f.png)

Lot 3, not surprisingly is a different scenario. Here the sample mean is 1496.14 and the p-Value is 0.04, which is lower than the common significance level of 0.05. All indicating to reject the null hypothesis that this sample mean and the presumed population mean are not statistically different.

## Study Design: MechaCar vs Competition


