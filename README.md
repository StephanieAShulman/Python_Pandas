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

[ALT !] PICTURE HERE

# Evidence of Academic Dishonesty (Challenge)
With concerns raised about results from Thomas High School 9th grade, the School Board has requested a repeat of the analysis, following replacement of the questionable scores. Deleting records or introducing zeros / missing values can upset mathematical operations. By replacing all reading and math scores with NaN (Not A Number), calculations can proceed without issue.

Thomas High School (THS), a charter school of 1,635 students, has 461 ninth graders who make up 28% of the population. The removal of these school would have a large impact at the school level, but – owing to the total number of student records analyzed (39,170) and to the coding techniques – any impact was indiscernible at the higher level.


