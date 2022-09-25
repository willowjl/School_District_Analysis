# School_District_Analysis

## Overview of the school district analysis
#### The school board contracted a data analysis due to some susoected academic dishonesty for Thomas High School. The reading and math scored for Thomas High School appear to have been altered. Even though the board did not know the full extend of the dishnoesty, they want to uphold state testing standards and have asked for help. 
### The data analysis was tasked to compare previous district analysis with the firm's data to assess how the suspected grades dishonesty may have affected school performance.

## Results
### How is the district summary affected?
#### The district summary is did not have a significant change after replacing 9th grade Thomas High School Student Data with NaN. The District Summary DataFrame is analyzing more than just data per each student, it analyzes data by overall school information (total schools, population of students, and total budget. Total Average Scores, Passing Scores, and Overall Passing Scores had some minor changes overall. The very small change which is a decrease in overall passing and average scores is most likely due to omitting the data that could have been falsified. 

### How is the school summary affected?
#### The school summary dataframe is affected in that after removing the false/altered data from the calculations, the scores drop overall for Thomas High School. When the falsified data was included, the scores were much higher for the percentage of those passing math, reading, and overall. When the data is excluded, the passing scores drop from the mid 90's to the mid 60's. This makes sense, given that the falsified/innacurate data would reflect a higher score overall and that the general scores would drop when the data is not counted. See the differences below in the two graphs (one for the original, and one that is filtered). This data is different because we have replaced the 9th grade reading and math scores at Thomas High School with NaN in the beginning of this analysis.

### How does replacing the ninth graders’ math and reading scores affect Thomas High School’s performance relative to the other schools?
#### Replacing the ninth graders' math and reading scores with Nan values clearly affects Thomas High School's performance relative to the other schools by showing that Thoma High School's freshmen are relatively struggling. The scores drop clearly when the innacurate data is excluded. For example, in the original code, when we sorted by top 5 schools, Thomas High School actually came in rated second. However, when substituting Nan for the inaccurate values, Thomas High School's % overall passing drops down around 65%, bringing it's standing compared to the other schools, much lower.

### How does replacing the ninth-grade scores affect the following:
### Math and reading scores by grade
####Replacing the ninth-graders scores affects the math and reading scores by grade simply by excluding the data for that column for that specific grade and that specific school. The data simply becomes Nan or null. All other data is left untouched for the other schools. Only Thomas High School is affected in the data that shows scores by grade. 

### Scores by school spending
####Replacing the ninth-graders scores does not actually affect the scores by schools spending because by the time we run this code, we will have replaced the overall Thomas High School passing scores in the dataframe with data for only the 10th through 12th grade and will not even count the ninth graders data in this analysis. So the scores by school spending dataframe remains unchanged. If we had caclulated this data before updating the frame to only show for 10th through 12th, the school spend per student would be much higher. I noticed in this code, that our challenge didn't ask us to update the dataframe for total students at Thomas High School to show as only 1,173 (1635 - 461 ninth graders). If the code had asked us to update our dataframe for total students from Thomas High School to be only 1,173 (10th Grade to 12th Grade Only), then the total spend per student would be much higher at $889.28 and would bump this school way up on the spending range per student.

### Scores by school size
####When we view the dataframes for scores by school size, we encounter the same phenomenon as we did in the last section (scores by spending), in that the data remains relatively unchanged from the first dataframe to the second, because we eliminated the ninth grader information from the average and passing scores, but the challenge code never asked us to update the total student number. For this reason, and because the 10th-12th graders had relatively the same scores as was counted in the original code with the inaccurate data of the 9th graders, we can see that there is really no difference of output below. Also the school size (even if we subtract the amount of 9th grader students), remains in the Medium Range(1,000 - 2,000)

### Scores by school type
####In this next section, we again see the same type of outcome that we saw in the previous two sections. The data remains unchanged in the scores by school type because again, we have eliminated the 9th grade null data, and replaced our datasets with only the passing grade info from 10th to 12th grade. If we left the dataset as affected by the null values, we would see a change in the scores, however at the end of the challenge code, we replaced this lower data, with info that shows just from the 10th-12th grades, which bring our scores back to the same as they were originally.

## Summary
### The first replacement of the 9th grade values with Nan bring down all the scores from Thomas High School across the board. But then, at the end of our code, we replace the school summary code with code that only counts the 10th-12th grade passing data. This brings our data back up. In our final dataframe therefore:
### The grades % increased for Thomas High School so it went from a low performing to a high performing school
### The % Passing Math Scores for Thomas High School returned back up to 93 from 66.9
### The % Passing Reading returned back up to 97 from 69.6
### The overall percentage of the passing returned back up to 90 from 65.
