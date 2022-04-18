# MechaCar_Statistical_Analysis

I was approached with a special project in the MechaCar, a prototype from AutosRUs'. I  helped Jeremy and the data analytics team do the following:

- Perform multiple linear regression analysis to identify which variables in the dataset predict the mpg of MechaCar prototypes
- Collect summary statistics on the pounds per square inch (PSI) of the suspension coils from the manufacturing lots
- Run t-tests to determine if the manufacturing lots are statistically different from the mean population
- Design a statistical study to compare vehicle performance of the MechaCar vehicles against vehicles from other      manufacturers. For each statistical analysis, you’ll write a summary interpretation of the findings.

## Resources

- R Studio 4.1.3

## Linear Regression to Predict MPG

After summarizing our MPG data:

![image](https://user-images.githubusercontent.com/96445453/163752113-d196bc77-7288-4f87-b223-980db185d51b.png)

- Which variables/coefficients provided a non-random amount of variance to the mpg values in the dataset?
  - According to our data vehicle_length(p-value 2.6 x 10^-12) and ground_clearance (p-value 5.21x10^-8) provide a non-random amount of variance to the mpg values in the dataset. The intercept is also a non-random amount of variance which may indicate additional data needed.

- Is the slope of the linear model considered to be zero? Why or why not?
  - The slope of the linear model is considered to be not zero. According to the data it has a p-value of 5.35x10^-11. The null hypothesis must be rejected as an extreme level of significance is shown. Our variables and the MPG is subject to more than random chance. 

- Does this linear model predict mpg of MechaCar prototypes effectively? Why or why not?
  - With a r-squared value of .7149 indicates our model being 71% accurate. With this model we can somewhat reliably predict the effectiveness of the Mechacar prototype.  

## Summary Statistics on Suspension Coils

After summarizing our Suspension Data:

![image](https://user-images.githubusercontent.com/96445453/163753868-beb10ae6-d7d6-49c0-a924-12b5ca8c3e58.png)
![image](https://user-images.githubusercontent.com/96445453/163753964-c2641c74-852d-4d39-afdd-93bbfdad1faa.png)

- Does the current manufacturing data meet this design specification for all manufacturing lots in total and each lot individually? Why or why not?
  - The total_summary data shows the overall variance is under PSI and within specifications. However on the lot_summary table the variance on Lot3 is over the acceptable threshold at 170.286.

 ## T-Tests on Suspension Coils
 
 Overall T-test results across all manufacturing lots and for each lot:
 ![image](https://user-images.githubusercontent.com/96445453/163755721-9673bae0-2183-43e7-8490-e64b12ac2f0d.png)

- The results of the suspension coils accross all manufacturing lots in this T-test shows a p-value of .06028 indicating the manufacturers are not statistically different from the population mean, this enough to reject the null hypothesis.

![image](https://user-images.githubusercontent.com/96445453/163755139-54b1680a-9aab-4586-9a4e-c837b2222410.png)

- The T-test results for Lot 1 shows a p-value of 1 indicating they are not statistically different from the population mean, therefor we can not reject the null hypothesis.

![image](https://user-images.githubusercontent.com/96445453/163755416-ecb6c84e-2ba4-4170-afc4-f4db3e35130c.png)

- The T-test results for Lot 2 suspension coils shows a p-value of .6072 and they are not statistically different from the population mean, therefor we can not reject the null hypothesis.

![image](https://user-images.githubusercontent.com/96445453/163755675-7718e69c-8928-4cf2-87b9-141cf976495e.png)

 - The T-test results for Lot 3 shows a p-value of .0417 and they are barely statistically different from the population mean, therefor we can reject the null hypothesis. Lot 3 needs to be looked at or discarded.

## Study Design: MechaCar vs Competition

