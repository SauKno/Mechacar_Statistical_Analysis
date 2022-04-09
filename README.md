# Mechacar_Statistical_Analysis
## D1: Linear Regression to Predict MPG
Q1. Vehicle_weight,spoiler_angle and AWD provide non random amount of variance. The maximum random variance was provided by ground_clearence and vehicle_length
Q2. Since p-value is less than zero (5.35e-11), the slope is not equal to zero.
Q3. The R squared value is 71.49% which implies that roughly 72% of the time the predictions will be correct using the linear model

<img width="814" alt="Screen Shot 2022-04-09 at 4 27 22 PM" src="https://user-images.githubusercontent.com/94129215/162590630-e17844e2-f2a3-4906-927f-65909389cfc5.png">
<img width="899" alt="Screen Shot 2022-04-09 at 4 27 45 PM" src="https://user-images.githubusercontent.com/94129215/162590634-e6e8861f-dcf8-412e-92bb-2091e0f81ae8.png">

## D2: Summary Statistics on Suspension Coils
First the Suspicion Coil csv was converted into a dataframe and then created two subset tables with it: Total Summary and Lot Summary. The Total Summary table examines the PSI Statistics of all the lots combined while the Lot Summary shows statistcs by each lot. ). As seen, Lot 1 and 2, are very similar while Lot 3 has a smaller mean with a bigger variance and standar deviation (SD).

<img width="1439" alt="Screen Shot 2022-04-09 at 4 36 30 PM" src="https://user-images.githubusercontent.com/94129215/162590833-9c6e3fd1-4ce9-4a5c-838d-69af96c955b4.png">
<img width="1437" alt="Screen Shot 2022-04-09 at 4 36 19 PM" src="https://user-images.githubusercontent.com/94129215/162590834-80414bd4-e0f1-4c9c-b48e-b98a5535fcf6.png">


## D3: T-Tests on Suspension Coils
The P-values from single T-Test on PSI values (compared to the standard of 1500 PSI) for suspicion coils:

All PSI= 0.06028 
Lot 1 PSI= 1 
Lot 2 PSI= 0.6072 
Lot 3 PSI= 0.04168 

Assuming that the significant value should be below p = 0.05 (which is standard), then only Lot 3 is significantly different. All other lots perform the same (or are not significantly different) to the standard 1500 PSI. This, combined with the lower mean of Lot 3 and high variance, could indicate that Lot 3 is under-performing.
<img width="807" alt="Screen Shot 2022-04-09 at 4 39 53 PM" src="https://user-images.githubusercontent.com/94129215/162590946-3cb8dc7b-c0ca-45b4-b546-2762bde306e3.png">

<img width="761" alt="Screen Shot 2022-04-09 at 4 40 06 PM" src="https://user-images.githubusercontent.com/94129215/162590955-fe225bdb-19e9-413d-9f45-73e905b22de6.png">

## Summary
Based on the analysis, the major impacts on MPG are car weight, spoiler angle, and AWD capability. Therefore, MechaCar designers and engineers need to consider these variables while determining improvements. In addition, when looking at suspension coils, Lot 3 has the most variance and lower PSI average. This could mean that Lot 3 should not be used within the MechaCar.

## Study Design: MechaCar vs Competition
For further analysis, the company should conduct an ANOVA test to compare the various categories that customers would care to compare: cost, city and highway fuel efficiency, horse power, safety rating, and maintenance cost. An ANOVA test is able to compare the means from multiple samples are significantly similar or different. If the p-value is greater than 0.05, then MechaCar has the same or similar performance within these categories (the null hypothesis). If the p-value is less than 0.05, then MechaCar is significantly different. If the hypothesis is proven to be true, then looking at MechaCar's averages to compare it to the competitors is the next step (below = worse, above = better)
