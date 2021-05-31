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
The School Summary reports statistics based on each school in the district. In the updated School Summary, we calculated the number of 10th-12th graders in Thomas High School and used this number to recalculate and replace the existing information around the students who passed math and reading for Thomas High School. As you can see below, there is very minimal change for Thomas High School and all the other schools' information remains the same. 

#### Original School Summary
![per_school_summary_original](/Resources/per_school_summary_original.PNG)

#### Updated School Summary
![per_school_summary_new](/Resources/per_school_summary_new.PNG)

## Summary
