# School_District_Analysis

## Resources
- Data Sources: students_complete.csv, schools_complete.csv
- Software: Python 3.7.6, Jupyter Notebook 6.4.5

## Project Overview
It's budget time again, and the School Board and Superintendent have relied on Maria, city school district Chief Data Analyst, and her team to provide pertinent information about the impact of school size, type and spending on standardized test scores. These scores in reading and mathematics reading provide a consistent measure across the various schools. Initial metrics of interest included:
- The district summary.
- The school summary.
- The top 5 and bottom 5 performing schools, based on the overall passing rate.
- The average math score for each grade level from each school.
- The average reading score for each grade level from each school.
- The scores by school spending per student, by school size, and by school type.

Using existing code to assist in the effort, two separate files were imported. After imputing missing values and removing incorrect data, the datasets were merged and used to product the School District Summary and the summary of individual school metrics, as well as the additional metrics.

![ALT Text](https://user-images.githubusercontent.com/30667001/149038072-daf46753-7feb-4d7d-b367-1c6421a45240.png)

## Evidence of Academic Dishonesty (Challenge)
With concerns raised about results from Thomas High School 9th grade, the School Board has requested a repeat of the analysis, following replacement of the questionable scores. Deleting records or introducing zeros / missing values can upset mathematical operations. By replacing all reading and math scores with NaN (Not A Number), calculations can proceed without issue.

Thomas High School (THS), a charter school of 1,635 students, has 461 ninth graders who make up 28% of the population. The removal of these school would have a large impact at the school level, but – owing to the total number of student records analyzed (39,170) and to the coding techniques – any impact was indiscernible at the higher level.

After replacing all of the 9th grade scores, the scores of the remaining 38,709 students were calculated. A new dataframe was created and the number of remaining THS students was calculated. These count of students (1,174 10th - 12th graders) became the basis of all remaining calculations. As a result, no other measures changed as the rest of the code was run.
- The district summary - no change
- The school summary
  - Even though this was run on the reduced number of students (n = 38,709), changes were imperceptible.
  - The overall passing percentage, for example, was modified from <INSERT> to 64.9%. Interestingly, not removing the 9th grade students (not required by provided code) would have resulted in an overall passing rate of 64.1%, likely due to the nature of NaNs as value-based entities.
- The top 5 and bottom 5 performing schools, based on the overall passing rate
  - No change
  - As all values were in similar ranges with and without the inclusion of 9th grade data, THS maintained its ranking at a Top 5 school by scores.
- The average math score for each grade level from each school - no change
- The average reading score for each grade level from each school - no change
- The scores by school spending per student, by school size, and by school type - no change
 
 ## Summary of Findings
  While there are likely multiple things that can occur when values are removed from a dataset, the use of NaN preserves the mathematics.
  Python appears to recognize it as a numerical value.
  Additionally, adjusting the denominator by including 10th through 12th graders only in the calculations preserved the existing scores and percentages as they were already in similar ranges.
 



