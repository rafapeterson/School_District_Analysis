# School_District_Analysis
## Analysis Overview
This is an analysis of 15 schools with a mixture of district & charter schools. The purpose of this analysis is to compare school performance based on school type, school size, and school spending (per capita). The analysis was then updated when (with guidance from the client) all ninth grade results from Thomas High School (THS) were removed.
## Results

* **How is the district summary affected?**<br/>
Because of the removal of the ninth grade data, THS's data is not as complete or accurate, compared to the data of other schools. As a result, any study on the school would need to be reviewed with the caveat of missing information regarding accurate reporting for grade 9 scores.

* **How is the school summary affected?** <br/>
The averages of passing in all three categories (math, reading, and overall) for THS only show the data of grades 10-12, thereby not painting as complete of a picture. This impacted the "% Passing Math, % Passing Reading, & % Overall Passing" categories. 

* **How does replacing the ninth graders’ math and reading scores affect Thomas High School’s performance relative to the other schools?**<br/>
 The following is a screenshot from the original school summary DataFrame, showing THS's scores (the last columns) as ~67% passing math, ~70% passing reading, and ~65% passing overall. ![image](https://user-images.githubusercontent.com/13009587/136251096-d1f40797-f2d5-4589-99c5-b27538fd0547.png) <br/> Once the data was adjusted to not account for grade 9, these were the results: ![image](https://user-images.githubusercontent.com/13009587/136251402-f35f33f6-2267-4f17-abbf-c6fa397703cd.png)<br/>
As you can see, the averages all shot up drastically. This also led to Thomas High School being listed in the top 5 schools.<br/> ![image](https://user-images.githubusercontent.com/13009587/136252898-8aa6e4b9-a116-44ed-84b3-929c8e5f863f.png)
<br/> In future analysis, capturing the accurate performance data for THS would be essential to be able to provide the most accurate analysis possible.  <br/>

* How does replacing the ninth-grade scores affect the following:
  * Math and reading scores by grade<br/>
  The results for Thomas High School's ninth grade is reflected as "NaN" when looking at performance based on grade. This only affects the result for 9th grade at Thomas High school, so the effect is minimal.
  ![image](https://user-images.githubusercontent.com/13009587/136253267-45a11bc9-fd3a-4372-a9e7-39a3a49b5961.png) <br/>

  * Scores by school spending<br/>
  The results for scores by school spending are more impacted than the scores by grade. The amount of money per student was not affected, as the "per student budget" was calculated prior to reducing the student count. However as stated previously, the percentages are still not fully indicative of the entire school's performance.
  * Scores by school size<br/>
  The results based on school size were similarly impacted. While school size category did not change, since the omission of Grade 9 reduced the total school size from ~1600 to 1174. This kept the school in the bin of "1000 to 2000 students," ![image](https://user-images.githubusercontent.com/13009587/136254196-89737607-21d0-454d-adcc-d3da973bba3b.png)<br/>
  the percentages are, as mentioned previously, not accurate without the inclusion of the actual results for grade 9. The impact is less than in other categories, but is still worthy of mention.<br/>
  
  * Scores by school type <br/>
  The results for this category would also be impacted by the lack of full results for Thomas High School, but as Charter Schools are in the majority of the data reviewed, its impact is less in this category than in others previously discussed.
  
  ## Summary 
  In summary, the following four changes were evident due to the replacement of ninth grade scores with NaNs:
  1) The percentages for passing reading, math, and overall passing were all impacted.
  2) Subsequently the inclusion of Thomas High School in the "Top 5 Schools" would not have occurred without removing the ninth grade scores
  3) Also, the scores by school spending were affected by the removal of the scores.
  4) The impact to the scores by school type were less than other categories due to the amount of charter schools reviewed.

Overall, this analysis demonstrates the impact editing data can have on a larger scale. This is important to pay attention to, as the decision to remove the data (rather than use compromised data) must be taken very seriously with the understanding of the rammifications of editing data sets.
