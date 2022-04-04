# PyCity School District Data Analysis

## Overview of Project

### Purpose
Maria is a data analyst that is tasked with finding trends and patterns through different data formats. In this case, we have been hired to assist in analyzing the data gathered from PyCity School system in regards to standardized testing, school size and type, and budgeting.  Through cleaning data, organizing, and combining like categories, we will be able to clearly provide the school district with any information on trends and correlations. We discovered that there was some falsification of grade results for a certain grade at one school and need to alter the code to accurately account for the removed scores.

## Analysis of Falsified Data Alterations
Initially we had analyzed the complete data provided by school and student data to compare things such as percent of passing grades to school size, budget allocation, and school types. Once we were informed of academic dishonesty in the 9th grade class of Thomas High School. With removing the falsified data, there was an impact to the overall data we will provide to the school system.

o	How is the district summary affected?

The following image is the DataFrame prior to removal of Thomas High School 9th Grade data:

![school type before](https://user-images.githubusercontent.com/100329223/161460404-2b64f6fb-e2ba-4412-8fd6-f6752fe36ff5.png)

The following image is the DataFrame prior to removal of Thomas High School 9th Grade data:

![school type after](https://user-images.githubusercontent.com/100329223/161460425-c1c3557c-c387-4215-a45b-4ee762e665c8.png)

Thomas High school is a Charter school type so the district school type data was not impacted.  Thomas High School was small enough that there was minimal impact to the data. After formatting, and rounding to the nearest integer, there appeared to be no impact at all. The values were impacted by removing the 9th grade students from the overall count and the averages of all student scores. 

o	How is the school summary affected?

The following image is the DataFrame prior to removal of Thomas High School 9th Grade data:

![summary before](https://user-images.githubusercontent.com/100329223/161463019-6020b000-a2f2-453a-b077-103d11558f8f.png)

The following image is the DataFrame prior to removal of Thomas High School 9th Grade data:

![summary after](https://user-images.githubusercontent.com/100329223/161463038-452b8b5a-858a-4332-91f4-0b2a2b720e10.png)

The school summary is impacted in a couple categories, where some categories were no impacted. First of all, the number of students did not change. The removal of data doesn’t negate the fact that the students still attended school there. The total school budget and per student budgets were also not impacted.  The average math and reading scores were altered by removing the falsified data, and reducing the number of students to account for the scores removed. One example of change in scores due to the removal of 9th grade Thomas High School data was the overall passing percentages. Prior to removal, the score was 90.948% of student with passing reading and math scores. Following the removal, this value dropped to 90.630%.

o	How does replacing the ninth graders’ math and reading scores affect Thomas High School’s performance relative to the other schools?

Ultimately, the adjustment for removing the 9th grade data, didn’t have too much of an impact on the comparison to other schools. Throughout the school system, test results from grades 9th to 12th only slightly varied within a school. The test scores between different schools did change, but were not impacted by the exclusion of a single grade within a certain school.

o	How does replacing the ninth-grade scores affect the following:

	Math and reading scores by grade, scores by school spending, scores by school size, scores by school type

By replacing the falsified values with a blank value, this would impact the average scores and percentages. In order to portray the most accurate results, we needed to adjust the number of students that contributed to the data set. The most inclusive example would be the overall passing score percentage prior to removing the falsified data is 90.948% and following the removal it was 90.630%. Similarly, scores by school spending, scores by school size, and schools by school type were not remarkably different comparing the results prior to removal, and after. If we wouldn’t have adjusted the number of students in average and percentage calculations, Thomas High School would not have appeared to perform well in the overall comparison between schools. 

## Conclusion
After refactoring the data to account for score falsification in the 9th grade students of Thomas High School, we came to the overall conclusion that the removal of this data, although not ideal, did not have a remarkable impact in its final numbers. The reading scores for Thomas High School went from an average score of 83.848 to 83.896. The math scores for Thomas High School went from an average score of 83.418 to 83.350.  The percent of passing scores for reading went from 97.309% to 97.019% and the percent of passing scores for math went from 93.272% to 93.186%. Overall passing percentages before the removal was 90.948% and following removal was 90.630%. When grouping similar items like school type of charter and spending ranges per student, the results of averages and percentages will be impacted but like previously mentioned, the adjustments were so minimal that it wouldn’t impact rankings or any other comparisons.
