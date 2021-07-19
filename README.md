# School District Analysis

## Overview
In this project, I analyzed the math and reading test scores of highschoolers throughout a school district with 15 schools. Through my analysis, I was able to compare the results in many different fashions:

- A school district summary showing the total number of schools and students; the total annual budget; the average math and reading scores amongst all students, as well as the percentage of students passing math, reading, and both tests.
- A per school summary showing the same information above, but breaking apart the results to show the performance of each high school. The budget per student was also calculated per each student.
- Finding the top and bottom 5 performing schools based on overall passing rate of both tests.
- The average math and reading test scores for each grade level at each school.
- The test scores by the amount of school spending per student.
- The test scores by school size.
- The test scores by school type, whether it be a charter or district school.

However, before I was able to gather all of this information, I needed to clean up the data since there was academic dishonesty found in 9th grade class of Thomas High School. I replaced all of their scores with "NaN" to ensure that cheating didn't influence the average scores and percentages district-wide.

## Results: Data
### School District Summary
#### The Original Data's District Summary
![](Resources/Old%20District%20Analysis.PNG)
#### The Refactored Data's District Summary
![](Resources/New%20District%20Analysis.PNG)

### School Comparison
#### The Original Data's School Summary
![](Resources/Old%20School%20Summary.PNG)
#### The Refactored Data's School Summary
![](Resources/New%20School%20Summary.PNG)

### Thomas High School Average Test Score Data
#### The Original Scores
![](Resources/Old%20Thomas%20High%20School.PNG)
#### The Refactored Scores (with the 9th Grade Scores removed)
![](Resources/New%20Thomas%20High%20School.PNG)

### The Refactored Math and Reading Scores by Grade
#### Old Math Scores
![](Resources/Old%20Math%20Scores%20by%20Grade.PNG)
#### New Math Scores
![](Resources/New%20Math%20Scores%20by%20Grade.PNG)
#### Old Reading Scores
![](Resources/Old%20Reading%20Scores%20by%20Grade.PNG)
#### New Reading Scores
![](Resources/New%20Reading%20Scores%20by%20Grade.PNG)

### Top and Bottom Performing Schools
#### Top 5 Schools
![](Resources/Top%205%20Schools.PNG)
#### Bottom 5 Schools
![](Resources/Bottom%205%20Schools.PNG)

### Test Scores by School Spending
![](Resources/New%20Spending%20per%20Student.PNG)

### Test Scores by School Size
![](Resources/New%20School%20Size.PNG)

### Test Scores by School Type
![](Resources/New%20School%20Type.PNG)

## Results: Analysis
With all of this data, it can be easy to overlook what changed when I refactored it. Below is a list of the main changes that occurred when I removed the 9th grade test scores from the dataset:
- When looking at the district analysis, the average math score decreased by 0.1, the The percent of students passing math decreased by 0.2%, the percent passing reading decreased by 0.1%, and the overall passing percentage decreased by 0.3%.
- In the school summary, only Thomas High School had any changes after I refactored the data:
  - The average math score decreased by about 0.06.
  - The average reading score increased by about 0.05.
  - The percent of students passing math decreased by about 0.09%.
  - The percent of students passing reading decreased by about .28%.
  - The overall passing rate of students for both tests decreased by about 0.32%.
- After refactoring the code, the changes to the overall passing rate were not greatly impactful, as they would still rank as the 2nd highest scoring school overall
- Replacing the ninth grade scores only affects the math and reading scores for Thomas High School. It especially affects the ninth-grade class at the school, which now has "NaN's" for their test scores now. If we had taken an average of all 9th grade test scores across all schools, removing the data would have likely decreased the average slightly, as Thomas High School's average is usually  a bit higher that other schools.
- The top 5 and bottom 5 schools were not affected by the refactored data.
- The test scores by school spending, school size, and school type were not affected after the refactoring.

## Summary
I was surprised to find that removing an entire grade's test scores from the dataset didn't change any of the data by all that much. Ther weren't any average scores or percentages that changed by more that 0.5 or 0.5%. This is likely because we had a large amount of data to begin with. While the changes weren't large, it is interesting to see how Thomas High School increases the test score averages for the entire district. It is unfortunate that some students cheated, as the rest of the class would have helped increase the district's overall metrics. 

At the district-level, the average math score decreased by 0.1 to 78.9. The average reading score did not decrease. The percentage of students passing math decreased by 0.2% to 74.8%. The percentage of students passing reading decreased by 0.1% to 85.7%. The overall passing rate for both tests decreased by 0.3% to 64.9%.
