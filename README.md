# School_District_Analysis

## Resources
- Data Sources: students_complete.csv, schools_complete.csv
- Software: Python 3.7.6, Jupyter Notebook 6.4.5

## Project Overview
It's budget time again, and the School Board and Superintendent have relied on Maria, city school district Chief Data Analyst, to provide pertinent information about the impact of school size, type and spending on standardized test scores. These scores in reading and mathematics provide a consistent measure across the various schools. Initial metrics of interest included:
- The district summary.
- The school summary.
- The top 5 and bottom 5 performing schools, based on the overall passing rate.
- The average math score for each grade level from each school.
- The average reading score for each grade level from each school.
- The scores by school spending per student, by school size, and by school type.

Existing code was used to assist Maria in this effort. Two separate files were imported. After imputing missing values and removing incorrect data, the datasets were merged and used to produce the School District Summary and the summary of individual school metrics, as well as the additional metrics.

![ALT Text](https://user-images.githubusercontent.com/30667001/149038072-daf46753-7feb-4d7d-b367-1c6421a45240.png)

## Evidence of Academic Dishonesty (Challenge)
With concerns raised about results from Thomas High School's 9th grade classes, the School Board requested a repeat of the analysis, following replacement of the questionable scores. Deleting records or introducing zeros / missing values can upset mathematical operations. By replacing all reading and math scores with NaNs (Not A Number), calculations could proceed without issue.

Thomas High School (THS), a charter school of 1,635 students, has 461 ninth graders who make up 28% of the population. The removal of these student grades would have a large impact at the school level, but – owing to the total number of student records analyzed (39,170) and to the coding techniques – an indiscernable impact at the district level.

After replacing all of the 9th grade scores, the scores of the remaining 38,709 students were calculated. A new dataframe was created and the number of remaining THS students was calculated. The count of these students (1,174 10th - 12th graders) became the basis of all remaining calculations. As a result, no other measures changed when the rest of the code was rerun.
- The district summary - no change
- The school summary
  - As comparison, overall passing for THS was 90.9% prior to removal of 9th grade scores. In an initial data run with the inclusion of NaNs, that score reduced to 65.1% (ie, fewer scores divided by the same number of students). When the 9th grade scores were removed and the data run on the remaining upperclassmen per instructions, the passage rate was basically the same (90.6%), due to the similarily of scores across all grades.
- The top 5 and bottom 5 performing schools, based on the overall passing rate
  - No change
  - As all values were in similar ranges with and without the inclusion of 9th grade data, THS maintained its ranking at a Top 5 school by scores.
- The average math score for each grade level from each school - no change
- The average reading score for each grade level from each school - no change
- The scores by school spending per student, by school size, and by school type - no change
 
 ## Summary of Findings
- While there are likely multiple things that can occur when values are removed from a dataset, the use of NaN preserves the mathematics. Python appears to recognize NaN as a numerical value.
- The removal of approximately one-third of the results from a school would have an enormous impact on totals and percentages if the denominator (full student count) were preserved. In this instance, however, the removal of the 9th graders from the count totals at the school level basically preserved existing scores and percentages as they were already in similar ranges. Any changes were at at the percentage level and of no consequence to rankings.
 



