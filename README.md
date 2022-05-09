# School District Analysis
School District Analysis using `Anaconda`, `Jupyter Notebook`, `Pandas` &amp; `Python`

## Overview of Project
Here is the list of deliverables for the analysis of the school district: 

* A high-level snapshot of the district's key metrics, presented in a table format
* An overview of the key metrics for each school, presented in a table format
* Tables presenting each of the following metrics:
    * Top 5 and bottom 5 performing schools, based on the overall passing rate
    * The average math score received by students in each grade level at each school
    * The average reading score received by students in each grade level at each school
    * School performance based on the budget per student
    * School performance based on the school size 
    * School performance based on the type of school
Before we can begin these tasks, we need to import the datasets into Jupyter Notebook using Python.

## Results
### How is the district summary affected?

**BEFORE CLEANUP**

- Average Math Score = **79.0**
- Average Reading Score = **81.9**
- % Passing Math **75**
- % Passing Reading **86** 
- % Overall Passing **65**
- 
**AFTER CLEANUP**

- Average Math Score = **78.9**
- Average Reading Score = **81.9**
- % Passing Math **74.8**
- % Passing Reading **85.7** 
- % Overall Passing **64.9**

**OBSERVATION:** From. what I can see the district summary is affected by a slight change in the Math Score, including % Passing district averages, Comparing the two dataframes above, the average show the difference when the 9th grade student Math and Reading scores from Thomas High Schools were excluded from the District Summary.


### How is the school summary affected?

**BEFORE CLEANUP**

- Thomas High School's % Overall Passing was **91**, placing second

**AFTER CLEANUP**

- Thomas High School's % Overall Passing was **65**, placing eight

**OBSERVATION:** The school summary is only affected the overall order change due to the cleanup,


### How does replacing the ninth graders math and reading scores affect Thomas High School’s performance relative to the other schools?

**OBSERVATION:** Replacing ninth graders math and reading scores affect Thomas High School’s performance between the other schools, Relative ranking for Thomas High School changed from 2nd place to 8th.

### How does replacing the ninth-grade scores affect the following:
- Analysis Below:

    * Math and reading scores by grade
        - Math and Reading Scores from Thomas High School 9th Grade set to "nan" and equivalent to 0.
        - Math and Reading Scores from Thomas High School 9th Grade means all of them failed (set to fail for analysis).
        - Doing that, the only significantly score affected was minimal in a very small in quantity. 
        - Student count() Before THS Cleanup was: 1635
        - Student count() After THS Cleanup was: 1174

    * Scores by school spending
        - Thomas HS is in the spending bucket "$630-644"
        - Math and Reading Scores from Thomas High School 9th Grade means all of them failed (set to fail for analysis).
        - Doing that, the only significantly score affected was minimal in a very small in quantity. 
        - Student count() Before THS Cleanup was: 1635
        - Student count() After THS Cleanup was: 1174
 
    * Scores by school size
        - Removing Thomas High School 9th Grade reduces the "% Passing Math", "% Passing Reading" and "% Overall Passing" scores for size bucket.

    * Scores by school type
        - Thomas High School is in the "CHARTER" type
        - Removing Thomas High School 9th Grade scores reduces the "% Passing Math", "% Passing Reading" and "% Overall Passing", see below.
    
  ## Summary
  After we have cleaning the data and replacing the scores of the 9th grade students, we are able to see that it has caused the scores to plummet. The district as a whole has also had its average math and reading scores decrease, as well as the overall passing percentage for students
