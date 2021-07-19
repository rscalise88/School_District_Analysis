# School_District_Analysis

## Overview of Project
Upon discovering that academic dishonesty may have affected the grades at Thomas High School, the test scores for the 9th grade class at Thomas High were nulled and the district-wide analysis of test scores was re-conducted based on the corrected data.

All data for 9th graders at Thomas High School within the data frame were nulled with the following blocks of code:

         thomas_9th_new_reading = student_data_df.loc[(student_data_df["grade"] == "9th") & (student_data_df["school_name"] == "Thomas High School"), ["reading_score"]] = "NaN" 
         thomas_9th_new_math = student_data_df.loc[(student_data_df["grade"] == "9th") & (student_data_df["school_name"] == "Thomas High School"), ["math_score"]] = "NaN" 
  
## Results
Upon running the updated script the account for the academmic dishonesty, we find the follow:
  - District-wide, we see a overall slight decrease in average scores and percentage of students passing both tests
![Original](https://github.com/rscalise88/School_District_Analysis/blob/main/Resources/SDA1.PNG)
![Updated](https://github.com/rscalise88/School_District_Analysis/blob/main/Resources/SDA2.PNG)

  - Thomas High's metrics also shifted down slightly when the grades were removed from the equation:
![Original](https://github.com/rscalise88/School_District_Analysis/blob/main/Resources/SDA3.PNG)
![Updated](https://github.com/rscalise88/School_District_Analysis/blob/main/Resources/SDA4.PNG)

  - Thomas High's standing in the distrct dropped significantly as a result of the change
    - Once ranked 2nd in the district, this school drops to 8th place due to the drop in overall scores.
    
  - Since the 9th grade scores were nulled, they are no no longer reflected in the graade-by-grade breakdown.  This has no effect on the statistics of the other grades
 
  - Among the schools that spend $630-644 per student, which contains Thomas High, the percentage of students passing both tests fell by 7%.
![Original](https://github.com/rscalise88/School_District_Analysis/blob/main/Resources/SDA5.PNG)
![Updated](https://github.com/rscalise88/School_District_Analysis/blob/main/Resources/SDA6.PNG)

  - Among medium-sized schools, which contains Thomas High, the percentage of students passing both tests fell by 6%.
![Original](https://github.com/rscalise88/School_District_Analysis/blob/main/Resources/SDA7.PNG)
![Updated](https://github.com/rscalise88/School_District_Analysis/blob/main/Resources/SDA8.PNG)

  - The effects were not seen as strongly ascorss school types, as there are only two. Nonetheless, the percentage of students passing at Charter Schools (Thomas High is a charter school), dropped by 3%.
![Original](https://github.com/rscalise88/School_District_Analysis/blob/main/Resources/SDA9.PNG)
![Updated](https://github.com/rscalise88/School_District_Analysis/blob/main/Resources/SDA10.PNG)

## Summary 
In brief: when the district-wide statistics are re-calculated to null all data for 9th-graders at Thomas High School, we see a decline in students who passed both tests for schools that are funded between $630-644, mid-sized schools (those with 1000-2000 students), and Charter Schools.  In addition, Thomas High's overall standing within the district drops signifcantly from 2nd in the disctrict, to 8th.
