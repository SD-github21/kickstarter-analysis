# Analysis of Kickstarter Campaigns for Theater Projects


## Overview of Project

### The purpose of this analysis is to provide a greater understanding of how well Kickstarter campaigns for different theater projects fared according to two key parameters, i.e., the date the campaign was launched and the fundraising goals set by the campaign. The results of this report are anticipated to provide information that will assist in decision-making processes regarding launching future Kickstarter campaigns, specifically for theater projects.


## Analysis and Challenges


### Analysis of Outcomes Based on Launch Date

#### A series of steps were completed to conduct an analysis of outcomes based on launch date. First, a "Year" variable was created in the Kickstarter table by entering the formula "=YEAR(S2)", where S2 referenced the column containing the "Date Created Conversion" data. This variable converted the date a campaign was launched into a simpler unit of data, i.e., the year the date occurred. Second, a pivot table was then initiated within Excel as the following images indicate:

![image](https://user-images.githubusercontent.com/85533099/130171754-5cf968bb-9060-4e9d-9b23-7b67960f1d26.png)

![image](https://user-images.githubusercontent.com/85533099/130171802-46241713-84a5-4cfe-8f6a-a12b8ca92ef2.png)

#### Next, options were selected within the pivot table in order to conduct the specific analysis requested. "Parent category" and "Year" were added under "Filters" and "Outcomes" was added under "Columns". Due to our specific interest in campaigns that were canceled, failed, and successful, a filter was initiated to only include these three specific categories of outcomes:  

![image](https://user-images.githubusercontent.com/85533099/130171868-3e157752-22cb-4077-b8e4-18953b11b190.png)

#### The variable "Years" was added under "Rows" and "outcomes" was added under "Values", with "Count of Outcomes" chosen as the specific value of interest. To conduct a more meaningful analysis, "Months" were utilized to showcase how campaigns fared according to their launch month. This was accomplished by removing two automatically generated variables in the "Rows" field, i.e., "Years" and "Quarters", which led to the final image depicted below where "Months" were visible in the Pivot Table:

![image](https://user-images.githubusercontent.com/85533099/130172085-bfacd21c-3e68-46dd-895a-5b87e9148190.png)

![image](https://user-images.githubusercontent.com/85533099/130172104-f362f45c-c086-4728-8fd8-6397847401c9.png)

![image](https://user-images.githubusercontent.com/85533099/130172134-f951ae77-8075-4ea6-bddc-a0b4b727f53d.png)

![image](https://user-images.githubusercontent.com/85533099/130172170-e0fbca3d-6d3c-49a3-b5f8-8ce2a4417ff7.png)

#### Two additional steps completed the analysis process. The "Parent Category" field was filtered to only include "theater" to view relevant Kickstarter campaigns for theater projects and the "outcomes" field was sorted in descending order to depict "successful", "failed" and "canceled" campaigns. Below are the corresponding images that detail these steps:

![image](https://user-images.githubusercontent.com/85533099/130172211-7251859f-6683-47e0-aac5-ec9781808421.png)

![image](https://user-images.githubusercontent.com/85533099/130172240-d88e1f46-b8e9-4390-a09e-513dd02d9fe4.png)

![image](https://user-images.githubusercontent.com/85533099/130172277-501255a8-3d64-4a28-a5af-abab1203b58d.png)

![image](https://user-images.githubusercontent.com/85533099/130172313-b127c9c4-9f57-492d-a2ef-c6724418e882.png)

#### Finally a pivot chart was created in order to gain a visual understanding of the relationship between launch month and outcomes. The following visuals depict the steps taken to ensure the pivot chart was created but that it also matched the exact targeted pivot chart used as a template in Canvas Module 1 (e.g., colors of the series were changed to red and yellow). A chart title was added as well:

![image](https://user-images.githubusercontent.com/85533099/130173313-926a3cb9-5986-401f-86f1-7d47d4440a9f.png)

![image](https://user-images.githubusercontent.com/85533099/130173325-4dfc24dc-ff8b-429c-bc2a-936ff7376c9c.png)

![image](https://user-images.githubusercontent.com/85533099/130173336-b7da8417-01f0-4023-827a-6e7a9b05b8cb.png)

![image](https://user-images.githubusercontent.com/85533099/130173350-9917ce11-2481-469b-b2c7-3ff9fd57c2ae.png)

![image](https://user-images.githubusercontent.com/85533099/130173374-f8051473-fc39-42ee-a00f-4a9a3e18e498.png)

![image](https://user-images.githubusercontent.com/85533099/130173387-0691fbf5-b828-4e47-bddb-8c2f8d36828b.png)

![image](https://user-images.githubusercontent.com/85533099/130173400-ab60673b-c0d1-4ca4-ad98-69da638afa25.png)

![image](https://user-images.githubusercontent.com/85533099/130173415-5fa2f4fa-92e8-4dcd-81cb-d25ef5d67457.png)

![image](https://user-images.githubusercontent.com/85533099/130173426-eb847463-006a-4023-a607-927a341e42be.png)

#### The Kickstarter data file and "Theater Outcomes Based on Launch Date" chart are attached as additional supporting documents to this report. 


### Analysis of Outcomes Based on Goals

#### A series of steps were completed to also conduct an analysis of outcomes based on goals. First, a new worksheet was created to hold data of interest, i.e., the number and percentage of successful, failed, and canceled theater projects. Goal ranges were added to the spreadsheet. The formula "=COUNTIFS(Kickstarter!$D:$D, "<1000",Kickstarter!$F:$F, "successful", Kickstarter!$R:$R, "plays")" was used to populate column B2 and then adjusted accordingly for columns C2 ("successful" was changed to "failed") and D2 ("successful" was changed to "canceled"). The copy function of hovering the cursor to the right of a cell to find the black “+” and then double-clicking to populate the column was utilized for efficiency:

![image](https://user-images.githubusercontent.com/85533099/130308500-fc831cf8-a78a-493e-82b4-be2fca725554.png)

![image](https://user-images.githubusercontent.com/85533099/130308509-6d6d4a5b-e34a-433e-8e4d-d565b74484de.png)

![image](https://user-images.githubusercontent.com/85533099/130308517-ceb6b965-967b-4c05-903a-0f010f0f9733.png)


#### Next, the formula "=SUM(B2:D2)" was entered and similarly copied  to fill in data for the "Total Projects" column:

![image](https://user-images.githubusercontent.com/85533099/130308524-27cd3eec-07f9-4d65-aadf-d62740dba426.png)


#### The last three columns, "Percentage Successful", "Percentage Failed", and "Percentage Canceled", were converted to a "Percentage" data format and then populated by the following formulas which were similarly copied down the columns: "=B2/E2", "=C2/E2", "=D2/E2". 

![image](https://user-images.githubusercontent.com/85533099/130308550-4ee42cb9-8594-4936-aa5b-5c9a55666118.png)

![image](https://user-images.githubusercontent.com/85533099/130308560-73e8cfb4-9a42-4798-b7da-ffb6a2f88ae6.png)

![image](https://user-images.githubusercontent.com/85533099/130308567-c2c1604b-fdf6-4f9a-990e-2f3e86113481.png)

#### Finally, a pivot chart was created in order to gain a visual understanding of the relationship between outcomes and goals. 

![image](https://user-images.githubusercontent.com/85533099/130308797-16de28c6-70d8-4cc5-b542-8ce67ddab44e.png)

![image](https://user-images.githubusercontent.com/85533099/130308800-1abbdf3b-9307-4e02-b47b-033ac4d3afc7.png)

#### The "Outcomes Based on Goals" chart is attached as an additional supporting document to this report. 

### Challenges and Difficulties Encountered

#### For the first analysis, I encountered a few challenges and difficulties. 
*At first, when I entered “Date Created Conversion” into the “Axis” box to create the Pivot Table, I could not figure out why I was seeing the years of the campaigns versus the months. Then I realized, as had been discussed in Module 1 in Canvas, that when I had added “Date Created Conversion” to the "Axis" box, there were two extra fields that were automatically added to that box and I had to delete them from the “Axis” box. When I deleted "Quarters" and "Years" and “Date Created Conversion” was the only variable remaining, Excel changed the date field to months automatically and I didn’t have to group the “Row Labels” column. When it came to sorting the campaign outcomes in descending order, I at first thought I had to do this in the "Kickstarter" worksheet. I sorted the "Outcomes" column in the "Kickstarter" worksheet in descending order and clicked back to the Pivot Table, but nothing changed. I thought I could only sort in the Kickstarter sheet since the Pivot Table was dependent on that sheet. I was stuck on this for a few moments. Then I realized that I could sort in the actual Pivot Table itself. 
*When it came to the Pivot Chart, I initially forgot how to save the chart into a separate file (which had been covered in Canvas Module 1). I at first thought I needed to move the chart into a new worksheet but realized this did nothing to actually create a ".png" file. Finally, I remembered the Microsoft Paint program that we used in Module 1 in Canvas and copied and pasted the chart. Afterwards, I checked to make sure that everything looked the same. I noticed that the default colors of my chart were orange for "Failed" and gray for "Canceled". "Successful" was the same color blue as the chart picture model in Canvas Module 1. It took me awhile to figure out how to change the colors. At first, I was changing the colors of the whole chart in the “Fill” and “Border” options. I couldn’t figure out how to change the line colors for quite some time. But then I clicked on the downward arrow next to Chart Options and this offered me options for ‘Series “successful”’, etc. When I clicked on the ‘Series’ options, I discovered I could then change the color of each of the lines so that they matched the colors in the Canvas Module model. 

#### For the second analysis, I wanted to see if I could intuit the “COUNTIFS” formula on my own without the hint offered by Canvas Module 1. I tried a formula using “AND” to separate the ranges of goals as well as to shorten the steps needed to complete the function. This was not successful. I explored the following two websites from a Google search on “COUNTIF” in Excel out of curiosity: 

#### https://exceljet.net/excel-functions/excel-countif-function
#### https://www.extendoffice.com/documents/excel/2412-excel-count-cells-between-two-values.html

#### I then also clicked on the video under “Show Hint” in Canvas Module 1. The combination of information from these sources assisted me in better understanding this function and permitted me to complete this task. I initially attempted to complete the “Percentages” columns by using the formula that we had learned in the Canvas Module 1 “=ROUND(B2/E2x100,0)”. I copied the same formula for all three “Percentages” columns. When I initially tried to run the Pivot Chart, the data was not showing up as it should. I was confused as to what was happening, until I realized that I had not formatted my data to be a “Number” field. Once I changed this, a Pivot Chart was created that looked like the model provided in Canvas Module 1. However, I noticed that my chart did not have “%” signs on the Y axis like that of the Canvas Module 1 picture, and this left me puzzled for awhile. During class, though, this issue was addressed, and I realized I could go into field lists and change data formats in Pivot Tables and Pivot Charts. However, when I tried to change the results to percentages in the Pivot Chart, I obtained numbers like 12000% on the axis instead of 120%. I realized the program was just multiplying the numbers by 100. Finally, I went back to the original spreadsheet “Outcomes Based on Goals” and reformatted the fields in the sheet itself. I changed my formula from the “=ROUND” into a fraction, i.e., “=B2/E2”. Then I changed the format of the cells to be “Percentages” and that appeared to solve the problem because the data converted to percentages in the columns for “Percentage Successful”, “Percentage Failed”, etc. When I clicked the Pivot Chart button, the chart automatically updated the Y Axis to percentages. It then looked exactly like the picture in Canvas Module 1.  

## Results

### Conclusions for “Outcomes based on Launch Date”
#### Two conclusions can be drawn from the analysis examining outcomes based on launch date. First, the data reveals that the launch months of May (n = 111) and June (n = 100) yielded the highest number of successful theater Kickstarter campaigns. Second, the launch months of November (n = 54) and December (n = 37) yielded the lowest number of successful theater Kickstarter campaigns. Thus, according to these results, it seems that theater Kickstarter campaigns launched in the months of November and December had a lower possibility of successful fundraising, while those that launched fundraising campaigns in either May or June had a greater possibility of successful fundraising. 
 

### Conclusions for “Outcomes based on Goals”
#### Conclusions can also be drawn from the analysis examining outcomes based on goals. First, 76% of the theater campaigns with a fundraising goal of “Less than $1,000” and 73% of the theater campaigns with a fundraising goal range of “1,000 to 4,999” were successful. Second, 80% of the theater campaigns with a fundraising goal range of “$25,000-$29,999” and 100% of the theater campaigns with a fundraising goal of “$45,000 -$49,999” failed. According to these results, it seems that theater campaigns that limited their budgets to less than $5,000 appeared to optimize their success with achieving their fundraising goals

### Limitations
#### For the first data analysis, the duration of time that a Kickstarter campaign ran from launch date to end date was not explored, representing an important limitation of our analysis. While we obtained a lot of information about optimal months to launch a campaign, the length of time people had to donate to the campaign would also likely be an important factor to consider. For example, campaigns might have failed because they had only been live for a month and this might not have provided enough time for interested backers to contribute to the campaign. For the second data analysis, it is interesting to note the variation in “Percentage Successful” for the different fundraising goal ranges. If it was truly the case that variables such as “Goal Range” of the project solely mattered, then we would have seen a linear decrease in success rate as the fundraising range increased. It is curious to note that 67% of theater campaigns that had fundraising goals of “$35,000-$39,999” and “$40,000-$44,999” were successful. This suggests that there are other factors influencing these trends and reveal limitations to our dataset. For example, audience’s familiarity with a play might be an important variable to consider, i.e., are there certain plays that are more popular to fund than others? In other words, are well-known plays that may be “fan-favorites” more likely to be funded? Are new plays with unknown playwrights harder to fund? Furthermore, would we glean more information knowing more data about the backers of these campaigns? What demographic constitutes backers most likely to donate to a campaign? For example, does relationship to the person starting the funding campaign matter, i.e., family members and friends versus individual donors with no personal relationship? Additionally understanding what constituted the project budgets might help to gain a better sense of which campaigns were more successful, i.e., what was the scale and scope of the projects and was this information included in the Kickstarter campaign details? Did some campaigns involve raising funds for the venues in addition to all the elements of putting on a play? It was mentioned in the Canvas Module that building a venue might have been included in a campaign. Our dataset does not contain any variables like this in the existing dataset. These are some areas of exploration that would help to flesh out a deeper understanding of why some plays with larger budgets were highly successful, while others with lower budgets were not. 

### Other possible tables and/or graphs of interest

#### As discussed above, I recommend examining the “Duration of campaign” and “Outcomes, where a new field “Duration of campaign” is generated by subtracting “Date Ended Conversion” from “Date Created Conversion”. “Duration of campaign” would provide the length of time that a campaign was live. The following link would be helpful to determine how to create this variable:
#### https://support.microsoft.com/en-us/office/calculate-the-difference-between-two-dates-8235e7c9-b430-44ca-9425-46100a162f38
#### Once this formula is created and copied down the column to generate the data, we can replicate the process utilized for our first data analysis examining “Launch Date” by “Outcomes” and obtain a graph examining “Duration of Campaign” by “Outcomes”. We could then know how campaigns fared according to how long they were allowed to remain active. Another recommended area of exploration with the existing dataset is to analyze data regarding “Average Donation” and answer the following question: Is there a relationship between “Average Donation” and “Outcomes”? In other words, were more successful campaigns those where the average donation was very high, indicating the important role of having influential backers or where the average donation was very low, indicating that having a large number of backers who could donate a small amount would be more beneficial? We can use a similar process utilized for our second data analysis examining “Goal Range” by “Outcomes” by creating dollar ranges for the “Average Donation” field and obtaining a similar visualization of the data according to these variables. This type of information might tell us how to go about engaging in outreach about our Kickstarter campaign, whether that would be to make sure that we have a solid network of people who could share our campaign online amongst their friends, families, and acquaintances or to consider approaching companies who might want to donate to our Kickstarter campaign and offer for them to receive some incentive,  such as advertising in our play programs that would be distributed to our audience members each night of the play’s performance as well as on our play's social media outlets.
