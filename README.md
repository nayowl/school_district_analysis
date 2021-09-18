# School District Analysis
## 1 Overview of The Project
School boards make decisions regarding the school budget and priorities. This project analyze data on student funding and student standardized test score to provide insights about school performance and trends. These insights will be used to inform discussions and strategic decisions at school and district level. 

In this project, it will include an analysis comparation of original data and data after replacement of reading and math score of 9th grader students in Thomas High School. Because there is evidence that shows academic dishonesty, the reading and the math score will be replaced by NaN. 

The following tasks will be performed in this analysis:
1.	Create and show district summary DataFrame.
2.	Create and show school summary DataFrame.
3.	Show top 5 performing schools, based on the overall passing rate
4.	Show bottom 5 performing schools, based on the overall passing rate
5.	Show average math score for each grade level from each school
6.	Show average reading score for each grade level from each school
7.	Show scores by school spending per student
8.	Show scores by school size
9.	Show Scores by school type
10.	Comparation before and after data replacement of Thomas High School

## 2 Resources
Data Sources: schools_complete. csv , students_complete.csv

Software: Python 3.7.6 , Jupyter notebook, Pandas library

## 3 Results 

To replace reading and math score for 9th grader students in Thomas High School to NaN,  .loc method will be used.  Figure 1 will show us the code in jupyter notebook to replace the code while Figure 2 will show us the result after the replacement.

![Figure 1 Code to Replace Nan](https://user-images.githubusercontent.com/88597187/133878454-de8035f6-fdaa-4d9a-89f0-9f78678ade8d.png)

<sub>Figure 1 Code to Replace Math and Reading Score to Nan </sub>
<p>&nbsp;</p>

![Figure 2 Results after alt](https://user-images.githubusercontent.com/88597187/133878463-0395b80d-a2e9-411f-93d3-f2ffcc008f62.png)

<sub>Figure 2 Results After Replacement  </sub>

To have better understanding of the impact after the replacement, here is the summary:
1.	District Summary

![Figure 3 Dist Sum Before Alt](https://user-images.githubusercontent.com/88597187/133878569-68054b3c-3a06-402f-96ae-9f10b7810099.png)

<sub>Figure 3 District Summary Before Replacement  </sub>
<p>&nbsp;</p>

![Figure 4 Dist Sum Aft Alt](https://user-images.githubusercontent.com/88597187/133878573-b7515477-7343-4002-9dfe-947279dd8fb5.png)

<sub>Figure 4 District Summary After Replacement  </sub>


Based on Figure 3 and Figure 4 above, there is  some difference in the district summary before and after replacement :

•	The average math score decreased 0.1 point to 78.9 from 79

•	The passing percentage for mathematic decreased 0.2% to 74.8% from 75%

•	The passing percentage for reading decreased 0.1% to 85.7% from 85.8%

•	The overall passing percentage for mathematic and reading decreased 0.3% to 64.9% from 65.2%





## 4 Summary
