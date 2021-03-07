# Kickstarter-Analysis
Performing analysis on Kickstarter data to uncover trends 


Then I wanted to populate columns that totalled the number of successful kickstarter campaigns that had the subcategory “plays” for each goal range. In order to populate the columns “Number Successful”, “Number Failed” I had to use the =countifs() function for each goal range. For example this is the formula used to populate the cell corresponding to “Number Successful” in the “<1000” goal range:
```
=COUNTIFS('Kickstarter Data'!$D:$D,"<1000",'Kickstarter Data'!$F:$F,"successful",'Kickstarter Data'!Q:Q,"plays")
```
I ran a similar formula for the “Number Failed” column, and then created the total projects column in order  to populate columns for “Percentage Successful” and “Percentage Failed”

<p align="center"

![alttext](https://github.com/sd2wiebe/Kickstarter-Analysis/blob/main/Outcomes_vs_Goals.png)

</p>
Background
Louise’s play Fever came close to its fundraising goal in a short amount of time. 
she wants to know how different campaigns fared in relation to their launch dates and their funding goals. 
visualize campaign outcomes based on their launch dates and their funding goals. 
# Kickstarting with Excel
## Overview of Project
The purpose of this analysis is to review and visualize data that will help my client Louise launch a successful fundraising campaign for her play, “Fever”. To aid Louise, I have looked at data points from successful and unsuccessful Kickstarter campaigns similar to hers, in order to give insight on the specific factors that might contribute to success or failure.
## Analysis and Challenges
1.	Analysis and Challenges: Explain how you performed your analysis using images and links to code, as well as any challenges you encountered and how you overcame them. If you had no challenges, describe any possible challenges or difficulties that could be encountered.
For this analysis I was able to use a large data set of Kickstarter campaigns with many variables, including: Goal amount, Launch Date, Outcome, Country, Category and Subcategory, and more.
The first thing I did was create a pivot table to summarize the data points I was interested in. I wanted to see if there was any correlation between the ‘Launch Date’ and whether the campaign was successful or not. The hope was to see if there was a specific launch month, or months that stood out as advantageous for a successful campaign. However, the data produced was still too vague, so I filtered the data in the pivot table to only show campaigns more similar to Louise’s. For this, I filtered to show only the kickstarters with subcategory “Theater” and based out of the United States. This proposed a challenge as the data set only had one column that displayed both category and subcategory. I was able to overcome this by creating two new columns and using the ‘Convert texts to Columns Wizard” to extract the parent category and the subcategory into the new columns respectively. Thus, I was able to create this pivot table:
[Link]
From the data in the pivot table, I created a line chart to visualize the relationship:
[Link]
We can see from the data in the pivot table that the biggest gap between the line indicating successful campaigns and the line indicating failed campaigns occurs in May and carries over into June. To further analyze this relationship, I made a new column that displays the percentage of successful campaigns for each month, along with the mean of those percentages and standard deviation.
[Link]
Two things are clear from this data. First, the highest number of campaigns are launched in May, June and July. Second, the highest success rates also occur in that three-month span, specifically in May (66.87%)
Conversely, December has the lowest total campaigns launched, and the lowest success rate by far (49.33%).
It is clear from this data that the optimal launch date for Louise’s Kickstarter campaign would be in May (66.87%) or June (65.36%).









### Analysis of Outcomes Based on Launch Date

### Analysis of Outcomes Based on Goals

### Challenges and Difficulties Encountered

## Results
When looking at project outcomes based on goal amount, we see that the highest success rates come with the lowest goal range. Less than 
 

1000$ has a success rate of 71.08%, the highest for any range. Conversely, we see the lowest success rate with our highest goal range, greater than 50,000$ with only 19.37%. 
Thus it is clear that the lower the goal, the higher the success rate. This makes sense because it should be easier to raise less money, thus making a smaller goal more attainable and likely to succeed.
- What are two conclusions you can draw about the Outcomes based on Launch Date?
Based on Launch date we can observe from the data that most campaigns were launched from May-Aug. and these months also corresponded with the highest success rates.



- What can you conclude about the Outcomes based on Goals?

- What are some limitations of this dataset?

- What are some other possible tables and/or graphs that we could create?

