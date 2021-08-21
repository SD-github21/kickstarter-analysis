# Analysis of Kickstarter Campaigns for Theater Projects


## Overview of Project

### The purpose of this analysis is to provide a greater understanding of how well Kickstarter campaigns for different theater projects fared according to two key parameters, i.e., the date the campaign was launched and the fundraising goals set by the campaign. The results of this report are anticipated to provide information that will assist in decision-making processes regarding launching future Kickstarter campaigns, specifically for theater projects.


## Analysis and Challenges


### Analysis of Outcomes Based on Launch Date

#### A series of steps were completed to conduct an analysis of outcomes based on launch date. First, a "Year" variable was created in the Kickstarter table by entering the formula "=YEAR(S2)", where S2 referenced the column containing the "Date Conversion Created" data. This variable converted the date a campaign was launched into a simpler unit of data, i.e. the year the date occurred. Second, a pivot table was then initiated within Excel as the following images indicate:

![image](https://user-images.githubusercontent.com/85533099/130171754-5cf968bb-9060-4e9d-9b23-7b67960f1d26.png)

![image](https://user-images.githubusercontent.com/85533099/130171802-46241713-84a5-4cfe-8f6a-a12b8ca92ef2.png)

#### Next, options were selected within the pivot table in order to conduct the specific analysis requested. "Parent category" and "Year" were added under "Filters" and "Outcomes" was added under "Columns". Due to our specific interest in campaigns that were canceled, failed, and successful, a filter was intiiated to only include these three specific categories of outcomes:  

![image](https://user-images.githubusercontent.com/85533099/130171868-3e157752-22cb-4077-b8e4-18953b11b190.png)

#### The variable "Years" was added under "Rows" and "outcomes" was added under "Values", with "Count of Outcomes" chosen as the specific value of interest. In order to conduct a more meaningful analysis, "Months" were utilized to showcase how campaigns fared according to their launch month. This was accomplished by removing two automatically generated variables in the "Rows" field, i.e., "Years" and "Quarters", which led to the final image depicted below where "Months" were visible in the Pivot Table:

![image](https://user-images.githubusercontent.com/85533099/130172085-bfacd21c-3e68-46dd-895a-5b87e9148190.png)

![image](https://user-images.githubusercontent.com/85533099/130172104-f362f45c-c086-4728-8fd8-6397847401c9.png)

![image](https://user-images.githubusercontent.com/85533099/130172134-f951ae77-8075-4ea6-bddc-a0b4b727f53d.png)

![image](https://user-images.githubusercontent.com/85533099/130172170-e0fbca3d-6d3c-49a3-b5f8-8ce2a4417ff7.png)

#### Two additional steps completed the analysis process. The "Parent Category" field was filtered to only include "theater" to view relevant Kickstarter campaigns for theater projects and the "outcomes" field was sorted in descending order to depict "successful", "failed" and "canceled" campaigns. Below are the corresponding images that detail these steps:

![image](https://user-images.githubusercontent.com/85533099/130172211-7251859f-6683-47e0-aac5-ec9781808421.png)

![image](https://user-images.githubusercontent.com/85533099/130172240-d88e1f46-b8e9-4390-a09e-513dd02d9fe4.png)

![image](https://user-images.githubusercontent.com/85533099/130172277-501255a8-3d64-4a28-a5af-abab1203b58d.png)

![image](https://user-images.githubusercontent.com/85533099/130172313-b127c9c4-9f57-492d-a2ef-c6724418e882.png)

#### Finally a pivot chart was created in order to gain a visual understanding of the relationship between launch month and outcomes. The following visuals depict the steps taken to ensure the pivot chart was created but that it also matched the exact targeted pivot chart used as a template (e.g., colors of the series were changed to red, yellow and blue):

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

#### A series of steps were completed to also conduct an analysis of outcomes based on goals. First, a new worksheet was created to hold data of interest, i.e., the number and percentage of successful, failed, and canceled theater projects. The formula "=COUNTIFS(Kickstarter!$D:$D, "<1000",Kickstarter!$F:$F, "successful", Kickstarter!$R:$R, "plays")" was used to populate column B2 and then adjusted accordingly for columns C2 ("successful" was changed to "failed") and D2 ("successful" was changed to "canceled"):

![image](https://user-images.githubusercontent.com/85533099/130308500-fc831cf8-a78a-493e-82b4-be2fca725554.png)

![image](https://user-images.githubusercontent.com/85533099/130308509-6d6d4a5b-e34a-433e-8e4d-d565b74484de.png)

![image](https://user-images.githubusercontent.com/85533099/130308517-ceb6b965-967b-4c05-903a-0f010f0f9733.png)


#### Next, the formula "=SUM(B2:D2)" was entered and copied to fill in data for the "Total Projects" column:

![image](https://user-images.githubusercontent.com/85533099/130308524-27cd3eec-07f9-4d65-aadf-d62740dba426.png)


#### The last three columns, "Percentage Successful" , "Percentage Failed", and "Percentage Canceled", were converted to a "Percentage" data format and then populated by the following formulas which were copied down the columns: "=B2/E2", "=C2/E2", "=D2/E2". 

![image](https://user-images.githubusercontent.com/85533099/130308550-4ee42cb9-8594-4936-aa5b-5c9a55666118.png)

![image](https://user-images.githubusercontent.com/85533099/130308560-73e8cfb4-9a42-4798-b7da-ffb6a2f88ae6.png)

![image](https://user-images.githubusercontent.com/85533099/130308567-c2c1604b-fdf6-4f9a-990e-2f3e86113481.png)

#### Finally, a pivot chart was created in order to gain a visual understanding of the relationship between outcomes and goals. 

![image](https://user-images.githubusercontent.com/85533099/130308797-16de28c6-70d8-4cc5-b542-8ce67ddab44e.png)

![image](https://user-images.githubusercontent.com/85533099/130308800-1abbdf3b-9307-4e02-b47b-033ac4d3afc7.png)

#### The Kickstarter data file and "Outcomes Based on Goals" chart are attached as additional supporting documents to this report. 


### Challenges and Difficulties Encountered

#### For the first analysis, I encountered a few challenges and difficulties. At first, when I entered “Date Created Conversion” into the “Axis” box to create the Pivot table, I could not figure out why I was seeing the years of the campaigns versus the months. Then I realized, as had been discussed in Module 1 in Canvas, that when I had added “Date Created Conversion” to the "Axis" box, there were two extra fields that were automatically added to that box and I had to delete them from the “Axis” box. When I deleted "Quarters" and "Years" and “Date Created Conversion” was the only variable remaining, Excel changed the date field to months automatically and I didn’t have to group the “Row Labels” column. When it came to sorting the campaign outcomes in descending order, I at first thought I had to do this in the "Kickstarter" worksheet. I sorted the "Outcomes" column in the "Kickstarter" worksheet in descending order and clicked back to the Pivot table, but nothing changed. I thought I could only sort in the Kickstarter sheet since the Pivot table was dependent on that sheet. I was stuck on this for a few moments. Then I realized that I could sort in the actual Pivot table itself. When it came to the Pivot Chart, I forgot how to save the chart into a separate file. I at first thought I needed to move the chart into a new worksheet, but realized this did nothing to actually create a "png" file. Finally, I remembered the Microsoft Paint program that we used in Module 1 in Canvas and copied and pasted the chart. Afterwards, I checked to make sure that everything looked the same. I noticed that the default colors of my chart were orange for "Failed" and gray for "Canceled". "Successful" was the same color blue as the chart picture in Module 1. It took me awhile to figure out how to change the colors. At first I was changing the colors of the whole chart in the “Fill” and “Border” options. I couldn’t figure out how to change the line colors for quite some time. But then I clicked on the downward arrow next to Chart Options and this offered me options ‘Series “successful”’, etc. When I clicked on the ‘Series’ options, I discovered Icould then change the color of the lines so that they matched the colors in the module. 


## Results

- What are two conclusions you can draw about the Outcomes based on Launch Date?

- What can you conclude about the Outcomes based on Goals?

- What are some limitations of this dataset?

- What are some other possible tables and/or graphs that we could create?

