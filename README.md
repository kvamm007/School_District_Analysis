# School District Analysis
## Project Overview
The purpose of this project was to analyze the data provided for the school district so they may better prepare for the next school year. The district needed to be able to see their overall performance (including student count & spending) as well as break outs by individual schools. They were also interested in seeing what sort of difference school size, spending per student, and school type made on the school performance. 

At some point, it was discovered within the district that there was a discrepancy with the 9th graders test scores, both math and reading, from Thomas High School. 9th grade scores from Thomas High School (THS) for math & reading were removed, and all summaries were refactored to reflect corrected averages. 

## Results
Below are comparisons of the data with the 9th graders from Thomas High School included & removed. The total number of students, total budget amounts & school types were not impacted by the removal of the students scores, as they were still counted as students at the school. 

- District Summary
  - Original:![District Summary- Original](https://user-images.githubusercontent.com/85597801/126916233-e7ddeb78-d598-48db-8724-2dea9d44c7d6.png)
  - Corrected: ![District Summary- corrected](https://user-images.githubusercontent.com/85597801/126916235-e0b65cc6-403a-4123-a381-f87c7fcfe1c9.png)

  - Average math score decreased by 0.1, average reading score remained the same. Passing math % decreased by 0.2%, passing reading percent decreased by 0.3% and overall     passing decreased by 0.1%. The largest difference is the decrease is passing reading.

- Schools Summary
  - Original: ![Schools- original](https://user-images.githubusercontent.com/85597801/126916242-68af47ce-7c30-42d1-8f81-ca15a37eb3a1.png)
  - Corrected: ![Schools- corrected](https://user-images.githubusercontent.com/85597801/126916247-c6747bbf-a0a2-4f97-8451-efbd6446e302.png)

  - The only school impacted was Thomas High School. The average math score decreased by 0.06 and the average reading score actually increased by 0.17. The percentage passing for math decreased by approximately 0.1%, the percentage passing for reading dropped by approximately 0.3%, and the overall percentage passing dropped by approximately 0.3%. As these are all less than 0.5 they would not impact the data if we were rounding, as is the case in some of the other outputs. 

- Comparison difference
  - Original:![Top 5 original](https://user-images.githubusercontent.com/85597801/126916255-9121b346-4e21-4f22-85b9-c56678f0ce5e.png)
  - Corrected: ![Top 5 corrected](https://user-images.githubusercontent.com/85597801/126916261-610babd9-d0c7-452c-9cc6-85859e26d2bf.png)

  - Thomas High School comes out as the #2 ranked school in the top 5 schools list both with and without the scores removed. The change in overall passing brought them (down) much closer to Griffin High School (they were up by about 0.34% and are now up by about 0.03%. Other schools would not be impacted in this view, unless the difference were big enough to move them up/down in the ranking of schools by overall passing percentage. 

- Math & Reading By Grade
  - Reading by Grade original: ![Reading by grade- original](https://user-images.githubusercontent.com/85597801/126916276-d5512260-5972-46db-adf2-c29c38a47d8e.png)

  - Reading by Grade corrected: ![Reading  by grade- corrected](https://user-images.githubusercontent.com/85597801/126916279-f60dd163-9ce6-4f13-8004-97547ece9f50.png)

  - Math by Grade original: ![Math by grade- original](https://user-images.githubusercontent.com/85597801/126916283-2711452b-8de2-4047-8503-ce34a313a4fa.png)

  - Math by Grade corrected: ![Math by grade- corrected](https://user-images.githubusercontent.com/85597801/126916290-97ff1721-d077-4897-a78a-038d52ded11c.png)

  - These are completely unchanged for all schools & grades besides Thomas High School, and 9th grade. This has changed from a listed score to “nan” meaning there was no value.

- Scores by school spending
  - Original: ![Spending ranges original](https://user-images.githubusercontent.com/85597801/126916317-6cd9c0fc-e554-4e87-b9d6-18dfd0622822.png)

  - Corrected: ![Spending ranges corrected](https://user-images.githubusercontent.com/85597801/126916320-7cc9b0a8-e241-4cf8-8d8b-d4e1158a1c5a.png)

  -  The differences were not large enough to be reflected in the data that is rounded to whole numbers, so any changes must have been very small. THS falls into the $630-$644 range, but there were no changes large enough to impact the whole numbers.

- Scores by school size
  - Original: ![Student Ranges- original](https://user-images.githubusercontent.com/85597801/126916401-542fe06e-b568-4b8a-8ec8-4a822c71dff4.png)

  - Corrected: ![Student ranges corrected](https://user-images.githubusercontent.com/85597801/126916302-5f84f647-4e3c-4dac-93ea-e5f2b3f7765c.png)

  - These also remain unchanged by the removal of THS data. THS would fall into the medium school size, 1,000-2,000 students, but none of the numbers there made a big enough difference to change with rounding. 

- Scores by school district type
  - Original: ![School types original](https://user-images.githubusercontent.com/85597801/126916324-c4a3fa69-2a79-4055-a5a3-f4e836d7f656.png)

  - Corrected: ![School types corrected](https://user-images.githubusercontent.com/85597801/126916326-02231c7c-4bb3-459f-a16d-d29d9fd9b9ad.png)

  - There was no difference in the school district type analysis with corrected scores, again with the averages and percentages being rounded. THS would fall into the “Charter” category but their score adjustment was not enough to impact this (they are one of 8 charter schools). 

## Summary of Changes

1.	THS itself was slightly impacted, with a slight decrease in average math, average percentage passing math, average percentage passing reading, and overall passing percentage; they actually saw a slight increase in their average reading scores. 
2.	The ranked order of school performance based on overall percentage of students that passed was not impacted by the adjustment, though THS was brought closer down to the #3 ranked school. 
3.	The school district totals were very slightly impacted; all are impacted by an amount that is small enough we likely would not see it if those numbers were rounded. 
4.	Due to rounding we are unable to see any changes in the school type, school size & school spending summaries, which means that any differences must be less than 0.5 or they would show up. This fits with the very small differences we saw in the longer, unformatted numbers. 

Since there were such slight (or no discernable) changes with so many of the scores, it is safe to assume that the questionable scores from THS 9th grade were distributed very close to the mean for the reading & math scores for the overall school. If we review the average math & reading scores for 9th grade at THS prior to them being removed, we can see they had an average score of 83.6 in math (corrected district average 78.9) and an average score of 83.7 in reading (corrected district average 81.9). So, combined with the other students at THS it made a slight difference, but district wide they only make up 1.18% of the district so it makes sense their scores would not have a large imapct, especially as they are close to the district averages. 
