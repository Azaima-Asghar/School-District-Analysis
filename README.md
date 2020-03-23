# School-District-Analysis:


## *PyCitySchools with Pandas*: 

## *Introduction*

Maria the chief data scientist for a city school district is responsible for analyzing information from a variety of sources in different variety of formats. In this role she is tasked with preparing all standardized test data for analysis, reporting and presentations that provide insight about performance trends and patterns. These insights are used to inform discussion strategic decisions at the school and district level. 

The aim of this project is to help Maria analyze data on student funding and students' standardized test scores. The data for the analysis includes every students' math and reading scores as well as various information about the schools they attend. 

The task of this analysis is to aggregate data and showcase trends and school performance. The analysis will assist the school board and super intendants in making decisions regarding the school budget and priorities based on the standardized test scores and current funding. The data are treated with utmost confidentiality to protect the students the reporting is based on.

## *Resources*
* Data Sources: school_complete.csv and student_complete.csv (present in the resources folder).
* Open-source distribution software Anaconda and the Jupiter notebook.
* Pandas Library for python.

## *Summary*

Initially, both the data sets (school and student) were cleaned, in student data student names were cleaned by removing the unique prefixes and suffixes from the student names. 

After the analysis was performed on data, a district and school summary DataFrames were created. Top and bottom five performing schools were also determined. The math and reading scores by grade, by school spending, by school size and by school type was also calculated along with the percentage overall passing. All these findings are present in "PyCitySChools. ipynb" file.

## *Challenge Overview*
Maria and her supervisor have discovered that the score averages for ninth graders from one high school are incorrect. The math and reading scores for Thomas High School for ninth-grade students are replaced with NaN using loc on student data.

## *Summary*

The district and school summary DataFrames are recreated. 

The district summary is very slightly changed, the average math and reading score changed very slightly where as the passing percentages dropped by 1 % after the addition of NaN for math and reading scores for Thomas High School. The following are the prominent changes:
* % Passing Math: 74.98	to 73.9
* % Passing Reading: 85.81 to 84.65	
* % Overall Passing: 65.17 to 64.10

For the school summary, values for all the other schools are just the same only values for Thomas High School changed. The average math and reading score changed slightly, but the passing percentages dropped drastically after the replacement of NaN for math and reading scores for Thomas High School. The major changes are the following:
* % Passing Math: 93 to 67
* % Passing Reading: 97 to 70
* % Overall Passing: 91 to 65

The high and low performing schools are recalculated.

Thomas High School was in the top five performing schools before the replacement of NaN for math and reading scores. After adding NaN values, it was no longer in the top five performing schools.

* Thomas High School dropped from second high performing schools to eighth position after replacing the ninth graders’ math and reading scores.

The scores by grade, scores by school spending, scores by school size, and scores by school type are recalculated.

 *Scores by grade*: Math score for 9th grade changed from 83.6 to nan, reading score changed from 83.7 to nan.

 S*cores by school spending*: The spending ranges per student are the same $630-644 for Thomas High School but there is a change in percentage passing math, reading and overall in the bracket of $630-644. The percentage passing math, reading and overall changed from 73, 84, 63 to 66, 77, 56 respectively.

 *Scores by school size*: Thomas High School falls in the category of a medium size (1000 - 2000) school. The percentage passing math, reading and overall changed for the school size. The percentage passing math, reading and overall changed from 94, 97 ,91 to 88, 91, 85 respectively. 

*Scores by school type*: The charter school type has the percentage passing math, reading and overall changed. The percentage passing math, reading and overall changed from 94, 97, 90 to 90, 93, 87 respectively.