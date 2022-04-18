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

