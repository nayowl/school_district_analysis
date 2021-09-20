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

To replace reading and math score for 9th grader students in Thomas High School to NaN,  .loc method will be used.  Figure 1 will demonstrates the code in jupyter notebook to replace the code while Figure 2 demonstrates the result after the replacement.

![Figure 1 Code to Replace Nan](https://user-images.githubusercontent.com/88597187/133878454-de8035f6-fdaa-4d9a-89f0-9f78678ade8d.png)

<sub>Figure 1 Code to Replace Math and Reading Score to Nan </sub>
<p>&nbsp;</p>

![Figure 2 Results after alt](https://user-images.githubusercontent.com/88597187/133878463-0395b80d-a2e9-411f-93d3-f2ffcc008f62.png)

<sub>Figure 2 Results After Replacement  </sub>

The following summary is presented to better understanding the impact after the replacement:

**1.	District Summary**

![Figure 3 Dist Sum Before Alt](https://user-images.githubusercontent.com/88597187/133878569-68054b3c-3a06-402f-96ae-9f10b7810099.png)

<sub>Figure 3 District Summary Before Replacement  </sub>
<p>&nbsp;</p>

![Figure 4 Dist Sum Aft Alt](https://user-images.githubusercontent.com/88597187/133878573-b7515477-7343-4002-9dfe-947279dd8fb5.png)

<sub>Figure 4 District Summary After Replacement  </sub>


Below are the differences found  in the district summary before and after replacement, based on Figure 3 and Figure 4 above, :

•	The average math score decreased 0.1 point to 78.9 from 79

•	The passing percentage for mathematic decreased 0.2% to 74.8% from 75%

•	The passing percentage for reading decreased 0.1% to 85.7% from 85.8%

•	The overall passing percentage for mathematic and reading decreased 0.3% to 64.9% from 65.2%


**2.School Summary**


![Figure 5 Sch Sum before Alt](https://user-images.githubusercontent.com/88597187/133891995-7dbcf9d2-350c-4b17-9255-d0aa8c52455d.png)

<sub>Figure 5 School Summary Before Replacement  </sub>
<p>&nbsp;</p>

![Figure 6 Sch Sum Aft Alt](https://user-images.githubusercontent.com/88597187/133892000-43787134-bed1-4a3d-b8d6-79b993d747bd.png)

<sub>Figure 6 School Summary After Replacement   </sub>

The school summary comparison will be focused on Thomas High School because there is no difference for the other school.  Listed below are the summary of the field affected by the replacement (The value will be rounded to 2 decimal):

•	The average math score decreased 0.07 point from 83.42 to 83.35 

•	The average reading score increased 0.05 point from 83.85 to 83.90  

•	The percentage passing math decreased 0.08% from 93.27% to 93.19%  

•	The percentage passing reading decreased 0.29%  from 97.31% to 97.02%

•	The overall passing percentage for mathematic and reading decreased  0.31% from 90.94% to 90.63%


**3.	School Performance**

![Figure 7 Sch Perform Bfr](https://user-images.githubusercontent.com/88597187/133892180-76662840-9d74-4a02-9c40-1cfd2e4f45c1.png)

<sub>Figure 7 School Performance Before Replacement   </sub>
<p>&nbsp;</p>


![Figure 8 Sch Perform Aft](https://user-images.githubusercontent.com/88597187/133892183-b51ba4cf-3840-480c-8958-8ac982f4ac82.png)

<sub>Figure 8 School Performance After Replacement   </sub>

The DataFrame from Figure 7 and Figure 8 display the top 5 high school performance based on the overall passing percentage of reading and math score. There is no difference on the order of the rank, even though there is a decrease of 0.32% in the overall passing percentage from before and after replacement. Thomas High School still the second highest performance in the list, because the other school do not surpass the overall passing percentage of Thomas High School.


**4.	Math and Reading Scores by Grade**


![Figure 9 Math Score by grade](https://user-images.githubusercontent.com/88597187/133892234-8064ccf7-fe28-40a6-b057-c76c39f313fa.png)

<sub>Figure 9 Math Scores by Grade Before and After Replacement   </sub>
<p>&nbsp;</p>

![Figure 10 Read Score by grade](https://user-images.githubusercontent.com/88597187/133892255-c17e4c0d-f80f-4823-a1b8-2eb8078e0e76.png)

<sub>Figure 10 Reading Scores by Grade Before and After Replacement </sub>

There is no change  for math and reading score for the other grade, as the scores are only altered for 9th Grader of Thomas High School. This statement is indicated by the 9th grade score on Figure 9 and and Figure 10 which has been altered to nan.


**5.	Scores by School Spending**


![Figure 11 School Spending bfr](https://user-images.githubusercontent.com/88597187/133892350-f60846e3-7b87-4dbb-9c8e-22ed8ea6f05f.png)

<sub>Figure 11 Scores by School Spending Before Replacement   </sub>
<p>&nbsp;</p>


![Figure 12 School Spending aft](https://user-images.githubusercontent.com/88597187/133892360-84f5d7ed-9f81-4157-b01b-51bd77537b10.png)

<sub>Figure 12 Scores by School Spending After Replacement </sub>

Figure 11 contains of two DataFrame before replacement of the Thomas High School data. The  DataFrame on top consists of non rounded values, while the DataFrame on the bottom is formatted to generate the rounded value. Figure 12 has the same format with Figure 11 with two DataFrame to display the data after replacement.

There is no difference found in the rounded up scores value of Figure 11 and Figure 12.However, some slight difference appears in the unrounded value of those figures, specifically in the scores and percentages between the before and after replacement of the data for spending ranges $630-$644( Thomas High School has spending ranges between $630-$644, hence it’s only impact in this range). For example, average math score is 78.518855 before the replacement and 78.502002 after the replacement. But because of the round up , the value become 78.5 for both before and after replacement.


**6.	Scores by School Size**


![Figure 13 school size bfr](https://user-images.githubusercontent.com/88597187/133892422-e52b1a2e-3022-4d26-a50b-917e12f5f711.png)

<sub>Figure 13 Scores by School Size Before Replacement  </sub>
<p>&nbsp;</p>

![Figure 14 school size aft](https://user-images.githubusercontent.com/88597187/133892424-030a2591-b18a-47a8-b72a-dceda8b4feee.png)

<sub>Figure 14 Scores by School Size After Replacement   </sub>

Figure 13 contains of two DataFrame before replacement of the Thomas High School data. The  DataFrame on top consists of non rounded values, while the DataFrame on the bottom is formatted to generate the rounded value. Figure 14 has the same format with Figure 13 with two DataFrame to display the data after replacement.

There is no difference found in the rounded up scores value of Figure 13 and Figure 14.However, some slight difference appears in the unrounded value of those figures, specifically in the scores and percentages between the before and after replacement of the data for school size Medium( Thomas High School is in Medium size , hence it’s only impact in this size). For example, average math score is 83.374684 before the replacement and 83.361201 after the replacement. But because of the round up the value become 83.4 for both before and after replacement.


**7.	Scores by School Type**


![Figure 15 school type bfr](https://user-images.githubusercontent.com/88597187/133892482-3c04465e-ec13-4e6d-b18c-2fb988538037.png)

<sub>Figure 15  Scores by School Type Before Replacement  </sub>
<p>&nbsp;</p>


![Figure 16 school type aft](https://user-images.githubusercontent.com/88597187/133892483-ffd329d3-e585-4451-8d88-dc8212a4d6d3.png)

<sub>Figure 16 Scores by School Type After Replacement  </sub>

Figure 15 contains of two DataFrame before replacement of the Thomas High School data. The  DataFrame on top consists of non rounded values, while the DataFrame on the bottom is formatted to generate the rounded value. Figure 16 has the same format with Figure 15 with two DataFrame to display the data after replacement.

There is no difference found in the rounded up scores value of Figure 15 and Figure 16.However, some slight difference appears in the unrounded value of those figures, specifically in the scores and percentages between the before and after replacement of the data for school type Charter( Thomas High School is in Charter type , hence it’s only impact in this type). For example, average math score is 83.473852 before the replacement and 83.465425 after the replacement. But because of the round up, the value become 83.5 for both before and after replacement.


## 4 Summary

The following is the changes in the school district analysis, based of the reading and math scores for 9th grades at Thomas High School which have been replaced with NaN:

•	District Summary 

There are some decrease in the average math score, the passing percentage for mathematic, the passing percentage for reading and the overall passing percentage after the replacement. The maximum difference is 0.3% for the overall passing percentage and the minimum is 0.1 for the average math score and 0.1% for the passing percentage for reading. The other field is not affected by the replacement. 

•	School Summary

There are some decrease in scores and percentages for average math score, percentage passing math, percentage passing reading and overall passing percentage after the replacement. The maximum the point or percentage decrease is in the overall passing percentage with 0.31 % and the minimum is the average math score with 0.07 point. There is also an increase in the average reading score with 0.05-point difference.

•	School Performance

The school performance is a rank of all the school based on the overall passing percentage. Although there is a change in percentage for Thomas High School after the replacement, Thomas High School rank is not changing at 2nd of the highest school performance. This is because the new value after the replacement is 90.630324% , while The 3rd  highest school performance overall passing percentage is 90.599455%.

•	Scores by Grade

There is no change in 10th-12th grade scores because the 9th grade students in Thomas High School are the only ones which have  of math and reading score value replaced to NaN. 

•	Scores by school spending, school size and school type

Although there are changes in scores by school spending in the range of $630-$644 , Medium School Size and Charter Type, the difference is too small. After the round up the value from before and after the replacement shows the same value. 
