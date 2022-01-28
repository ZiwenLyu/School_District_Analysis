# School District Analysis
## Overview of the school district analysis:
This project is to prepare standardized test data in the City School district for analyzing and reporting insights about student performances and trends. Those insights will assist school boards and superintendents in making decision of strategies, budgets, and other priorities. In the following analysis, we will first clean, merge, and group data to provide summaries of this district's, each school's and each grade's overall performance, then group schools based on their spendings, school sizes, and school types to discover any relations with their average scores and passing percentages. After the first analysis, we found out that Thomas High School's 9th grade had altered their math and reading scores, so we replace their grades with NaN but leave other data intact. We will explain how replaced data affect the overall analysis result.


## Result Comparison
### The District Summary
![The Distrcit Summary with THS 9th grade](https://github.com/ZiwenLyu/School_District_Analysis/blob/main/Resources/district_summary_1.png)
![The Distrcit Summary without THS 9th grade](https://github.com/ZiwenLyu/School_District_Analysis/blob/main/Resources/district_summary_2.png)
The first district summary with THS 9th grade got average math score of 79.0, average reading score of 81.9, 75.0% of math passing rate, 85.5% of reading passing rate, and 65.2% of overall passing rate. From the second district summary after taking out THS 9th grade, the average math score slides a bit to 78.9, the average reading score remains as 81.9, the math passing rate drops a little to 74.8%, the reading passing rate also decreases to 85.7%, and the overall passing rate goes down to 64.9%. 

### The School Summary
#### Replace THS 9th Grade Scores with NaN
![The School Summary with THS 9th grade](https://github.com/ZiwenLyu/School_District_Analysis/blob/main/Resources/school_summary_1.png)
![The School Summary without THS 9th grade](https://github.com/ZiwenLyu/School_District_Analysis/blob/main/Resources/school_summary_2.png)
The first school summary with THS 9th grade shows 15 schools's performance in average math grades, average reading grades, math passing percentages, reading passing percentages, and overall passing percentages. The second school summary replace all THS 9th grade's scores with NaN, we can see that its passing rates tumble a lot. Regarding to its overall passing rate, THS became one of the bottom five schools.

#### Re-calculate THS 10th-12th Grade Passing Rates
![The School Summary with THS 10th-12th passing rates](https://github.com/ZiwenLyu/School_District_Analysis/blob/main/Resources/top_school.png)
As the screenshot suggests, after we re-calculate THS 10th-12th grade's passing rates and update the school summary, THS becomes one of the top five schools in this district regarding to its overall passing rate. Its math passing percentages grows from 66.9% to 93.2%, reading passing rate increases from 69.7% to 97.0%, and overall passing rate goes up from 65.1% to 90.6%.

### Math and reading scores by grade 
This is every school's math and reading performances grouped by 9th-12th grade without replacing THS 9th grade score. 
![math scores by grade with THS 9th grade](https://github.com/ZiwenLyu/School_District_Analysis/blob/main/Resources/grade_summary_math1.png)
![reading scores by grade with THS 9th grade](https://github.com/ZiwenLyu/School_District_Analysis/blob/main/Resources/grade_summary_reading1.png)

This is every school's math and reading scores grouped by 9th-12th grade after replacing THS 9th grade score. We can see that THS 9th grade scores become NaN.

![math scores by grade without THS 9th grade](https://github.com/ZiwenLyu/School_District_Analysis/blob/main/Resources/grade_summary_math2.png)
![reading scores by grade without THS 9th grade](https://github.com/ZiwenLyu/School_District_Analysis/blob/main/Resources/grade_summary_reading2.png)

### Scores by school spending
This is school's math and reading performances grouped by their spendings(<$584, $585-629, $630-644, $645-675). The first pic is with THS 9th grade and the second pic replaces THS 9th grade. Basically, there is little or no change after altering the data. And suprisingly we find out that the spending is negatively relative to the overall passing rate.
![scores by spendings with THS 9th grade](https://github.com/ZiwenLyu/School_District_Analysis/blob/main/Resources/score_by_spending1.png)
![scores by spendings without THS 9th grade](https://github.com/ZiwenLyu/School_District_Analysis/blob/main/Resources/score_by_spending2.png)

### Scores by school size
This is school's math and reading performances grouped by their school sizes(Small (<1000), Medium (1000-2000), Large (2000-5000)). The first pic is with THS 9th grade and the second pic replaces THS 9th grade. Basically, there is little or no change after altering the data. And The school size is negatively relative to the overall passing rate.
![scores by school size with THS 9th grade](https://github.com/ZiwenLyu/School_District_Analysis/blob/main/Resources/score_by_size1.png)
![scores by school size without THS 9th grade](https://github.com/ZiwenLyu/School_District_Analysis/blob/main/Resources/score_by_size2.png)

### Scores by school type
This is school's math and reading performances grouped by their school types(District, Charter). The first pic is with THS 9th grade and the second pic replaces THS 9th grade. Basically, there is little or no change after altering the data. And apparently district schools have lower passing rates than charter schools.
![scores by school type with THS 9th grade](https://github.com/ZiwenLyu/School_District_Analysis/blob/main/Resources/score_by_type.png)
![scores by school type without THS 9th grade](https://github.com/ZiwenLyu/School_District_Analysis/blob/main/Resources/score_by_type2.png)

## Summary
After reading and math scores for the ninth grade at Thomas High School have been replaced with NaNs, we can see that the district score performance (average math) and passing rates (math passing rate, readig passing rate, and overall passing rate) all drop a little. If we only take THS's 10th-12th grade scores into the passing percentage, Cabrera High School, Thomas High School, Griffin High School, Wilson High School, and Pena High School are the top five schools; while Rodriguez High School, Figueroa High School, Huang High School, Hernandez High School, and Johnson High School are the bottom five schools. Scores grouped by grade, spendings, school sizes, and schools types aren't affected a lot by the data alteration. 
