# PyCitySchools with Pandas

## Overview of Project
For this week's project, we will be using Python and the Pandas Library in Jupyter Notebook. Pandas is an open-source Python library that is specific for data manipulation and analysis. Pandas contains very powerful data structures, such as Series and Dataframes, and can be used as a tool to analyze and clean data in the Python programming language. In additional to Pandas, we will be using Jupyter Notebook. Jupyter Notebook is a web-based application where you can write and execute live code to import, sort, and visualize data. This interactive tool is easy to use and is a great way to show and check the results quickly from your code. Using Pandas in Jupyter Notebook, we will be able to help others find trends and make strategic decisions based on our findings.

### Purpose
The purpose of this week's project was to help Maria, a chief data scientist for a school district, analyze standardized test data. Our goal was to assist Maria in finding trends in school performance and showcase this information to the school board and superintendent. This analysis helped provide insight on math and reading scores, school budgets, and different school performances per grade. After we imported the CSV data sets, calculated average scores and percentages, and created district and school summaries, we found alarming patterns in the data. In our original report, there were signs of academic dishonesty, specifically with Thomas High School ninth graders' scores. In order to uphold state-testing standards, we replaced the math and reading scores for the ninth graders at Thomas High School with NaNs (not a number) and reran the analysis for the school district.

## Results

### District Summary
The District Summary shows an overview of the school district's performance. We recalculated the data from the original District Summary by removing the number of Thomas High School's ninth grade students from the total student count. The updated District Summary below shows the recalculated student count, average math and reading scores, passing math and reading percentages, and overall passing percentage. Overall, there is very minimal change for the average scores and percentages even after removing 461 students from the total student count.

#### Original District Summary
![district_summary_original](/Resources/district_summary_original.PNG)

#### Updated District Summary
![district_summary_new](/Resources/district_summary_new.PNG)

### School Summary
The School Summary reports statistics based on each school in the district. In the updated School Summary, we first calculated the number of 10th-12th graders in Thomas High School. We then used this number to recalculate and replace the existing information around the students who passed math and reading for Thomas High School. As you can see below, there is very minimal change for Thomas High School and all the other schools' information remains the same.

#### Original School Summary
![per_school_summary_original](/Resources/per_school_summary_original.PNG)

#### Updated School Summary
![per_school_summary_new](/Resources/per_school_summary_new.PNG)

### Performance of Schools Based on Overall Passing Rate
Replacing the ninth graders' math and reading scores showed very minimal changes in our results. The updates overall did not affect Thomas High School's performance relative to other schools. Thomas High School remains in the top 5 performing schools. The bottom 5 schools have not changed. 

#### Original Top 5 Performing Schools
![top_five_original](/Resources/top_five_original.PNG)

#### Updated Top 5 Performing Schools
![top_five_new](/Resources/top_five_new.PNG)

#### Original Bottom 5 Performing Schools
![bottom_five_original](/Resources/bottom_five_original.PNG)

#### Updated Bottom 5 Performing Schools
![bottom_five_new](/Resources/bottom_five_new.PNG)

### Math and Reading Scores by Grade
The biggest change of results is shown below because it is based by grade. Since we were only replacing 9th graders from Thomas High School's scores with NaN, you can see that value changed for both reading and math. The rest of the data in the file is the same because we did not update or replace that data. 

|Original Math Scores by Grade     |Updated Math Scores by Grade      |
|------------|-------------|
|![math_scores_by_grade_original](/Resources/math_scores_by_grade_original.PNG)|![math_scores_by_grade_new](/Resources/math_scores_by_grade_new.PNG)|


|Original Reading Scores by Grade     |Updated Reading Scores by Grade      |
|------------|-------------|
|![reading_scores_by_grade_original](/Resources/reading_scores_by_grade_original.PNG)|![reading_scores_by_grade_new](/Resources/reading_scores_by_grade_new.PNG)|


### Other Results
The other results such as scores by school spending per student, score by school size, and scores by school type had the least changes after replacing Thomas High School's ninth grade scores.

#### Scores by School Spending
Thomas High School falls under the $630-644 spending range per student. As you can see from the summary of spending ranges, there are unnoticable changes after the update. 
##### Original Scores by School Spending Per Student
![spending_ranges_original](/Resources/spending_ranges_original.PNG)

![spending_summary_original](/Resources/spending_summary_original.PNG)

##### Updated Scores by School Spending Per Student
![spending_ranges_new](/Resources/spending_ranges_new.PNG)

![spending_summary_new](/Resources/spending_summary_new.PNG)

#### Scores by School Size
Thomas High School falls under the Medium (1000-2000) school size category. There is little to no change after the update. 
##### Original Scores by School Size Summary
![size_summary_original](/Resources/size_summary_original.PNG)

##### Updated Scores by School Size Summary
![size_summary_new](/Resources/size_summary_new.PNG)

#### Scores by School Type
Thomas High School is a Charter school type. There is little to no change after the update for both school types.
##### Original Scores by School Type
![type_summary_original](/Resources/type_summary_original.PNG)

##### Updated Scores by School Type
![type_summary_new](/Resources/type_summary_new.PNG)

## Summary
After replacing the Thomas High School's ninth grade scores, there was very minor changes in our results. Only 461 students had their reading and math scores changed to NaN which is very small percentage of the total student count. Here are a few changes in the updated school district analysis:
- We no longer have the average of math and reading scores for ninth grade students at Thomas High School and they are replaced with NaN
- In the District Summary, the passing math and reading percentages decreased:
		- Passing Math %: 75.0% to 74.8%
		- Passing Reading %: 85.8% to 85.7%
- The overall passing percentage in the District Summary decreased slightly from 65.2% to 64.9%
- For Thomas High School, the overall passing percentage decreased slightly from 90.9% to 90.6%
