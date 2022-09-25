# School_District_Analysis

## Overview of the school district analysis
### The school board contracted a data analysis due to some susoected academic dishonesty for Thomas High School. The reading and math scored for Thomas High School appear to have been altered. Even though the board did not know the full extend of the dishnoesty, they want to uphold state testing standards and have asked for help. 
### The data analysis was tasked to compare previous district analysis with the firm's data to assess how the suspected grades dishonesty may have affected school performance.

## Results
### How is the district summary affected?
### The district summary is did not have a significant change after replacing 9th grade Thomas High School Student Data with NaN. The District Summary DataFrame is analyzing more than just data per each student, it analyzes data by overall school information (total schools, population of students, and total budget. Total Average Scores, Passing Scores, and Overall Passing Scores had some minor changes overall. The very small change which is a decrease in overall passing and average scores is most likely due to omitting the data that could have been falsified. 

### How is the school summary affected?
### The school summary dataframe is affected in that after removing the false/altered data from the calculations, the scores drop overall for Thomas High School. When the falsified data was included, the scores were much higher for the percentage of those passing math, reading, and overall. When the data is excluded, the passing scores drop from the mid 90's to the mid 60's. This makes sense, given that the falsified/innacurate data would reflect a higher score overall and that the general scores would drop when the data is not counted. See the differences below in the two graphs (one for the original, and one that is filtered). This data is different because we have replaced the 9th grade reading and math scores at Thomas High School with NaN in the beginning of this analysis.

### How does replacing the ninth graders’ math and reading scores affect Thomas High School’s performance relative to the other schools?

### How does replacing the ninth-grade scores affect the following:

### Math and reading scores by grade

### Scores by school spending

### Scores by school size

### Scores by school type

## Summary
### The first replacement of the 9th grade values with Nan bring down all the scores from Thomas High School across the board. But then, at the end of our code, we replace the school summary code with code that only counts the 10th-12th grade passing data. This brings our data back up. In our final dataframe therefore:
### The grades % increased for Thomas High School so it went from a low performing to a high performing school
### The % Passing Math Scores for Thomas High School returned back up to 93 from 66.9
### The % Passing Reading returned back up to 97 from 69.6
### The overall percentage of the passing returned back up to 90 from 65.
