# Analysis of Relevant Kickstarter Campaigns

## Overview of Project

### The purpose of this analysis is to provide a greater understanding of how well Kickstarter campaigns for different theater projects fared according to two key parameters, i.e., the date the campaign was launched and the fundraising goals set by the campaign. The results of this report are anticipated to provide information that will assist in decision-making processes regarding launching future Kickstarter campaigns, specifically for theater projects.

## Analysis and Challenges

### Analysis of Outcomes Based on Launch Date

#### First, a "Year" variable was created in the Kickstarter table by entering the following formula: =YEAR(S2), where S2 referenced the column containing the "Launch Date" data. This variable allowed for a conversion of data from the date a campaign was launched into a simpler unit of data, i.e. the year the date occurred. Second, a pivot table was then initiated within Excel:

![image](https://user-images.githubusercontent.com/85533099/130137714-ce871209-0e80-4f3e-9c37-781852f0df6c.png)

![image](https://user-images.githubusercontent.com/85533099/130137792-29b3d93c-94a2-4159-b886-fafcc6bfdd3d.png)

#### Next, options were selected within the pivot table in order to conduct the specific analysis of interest. Parent category and Year were added as Filters and Outcomes were added as "Columns". Due to our specific interest in campaigns that were canceled, failed, and successful, a filter was intiiated to only include those specific categories of outcomes:  

![image](https://user-images.githubusercontent.com/85533099/130138581-3b67f8a3-e67f-4754-a80f-8fd77c2cf0b1.png)

#### The variable "Years" was added as "Rows" and "outcomes" was added as "Values", with "Count of Outcomes" chosen as the specific value of interest. 







### Analysis of Outcomes Based on Goals

### Challenges and Difficulties Encountered

## Results

- What are two conclusions you can draw about the Outcomes based on Launch Date?

- What can you conclude about the Outcomes based on Goals?

- What are some limitations of this dataset?

- What are some other possible tables and/or graphs that we could create?

