# Kickstarter-analysis
Performing analysis on Kickstarter data to discover trends

## Overview of Project
### Purpose
Analyze Kickstarter funding campaign data to discover how different campaigns have fared in relation the their launch dates and their funding goals.

## Analysis and Challenges

### Analysis of Outcomes Based on Launch Date
The Kickstarter dataset includes data for a variety of activity categories, such as games, music, technology, and theater, as examples. 

Using Excel pivot tables and filters, I used the data for "theaters" to analyze the campaigns based on their launch dates. The launch dates were converted to a standard date format in the dataset, sorted by months, and then counted by the standard outcomes of successful, failed or canceled. 

Using a line chart showing the months of the calendar year, the number of campaigns by outcome are shown by month.  
![Outcomes Based on Launch Date]()

### Analysis of Outcomes Based on Goals
Under the theather category, there are three subcategories or types of projects in the Kickstarter data: musicals, plays and spaces. Also, the funding goals of the campaigns cover amounts between $1.00 to $30 million. 

In order to analyze the data based on the funding goal of the campaigns, I sorted the funding goals into ranges of amounts and then counted the number of campaigns by their outcome - successful, failed, or canceled - for each range of funding goal. The counts were then converted to percentages of the total number of projects in that range. 

Using another line chart, the percentage of campaigns with specific outcomes is shown for each funding range group.
![Outcomes Based on Goals]()

### Challenges and Difficulties Encountered
I encountered two challenges in preparing the data for analysis. 

The first was getting the date of campaigns to show by Month. The Date Created Converted data kept displaying in Quarters. I had to regroup that data to get display the Months.

The second was in editing the COUNTIFS formulas as I copied them throughout the different cells. I ended up adding $'s to the columns in the Kickstarter dataset to hold the formuals steady for each outcome. So my initial formula for successful outcomes looked like this: =COUNTIFS(Kickstarter!$F:$F,"successful",Kickstarter!$D:$D,"<1000",Kickstarter!$R:$R,"plays"). From there, I only had to manually edit the funding amount range in the cells below. I did the same for the other outcome columns.

## Results

- What are two conclusions you can draw about the Outcomes based on Launch Date? 

While it is possible to have a successful Kickstarter funding campaign for a theater project during any month of the year, more campaigns have been successful that launched during May, June or July.

The liklihood of success or failure for Kickstarter theater funding campaigns launched in December has been about equal, with roughly the same number of campaigns failing and succeeding to meet their goals.

- What can you conclude about the Outcomes based on Goals?

Kickstarter funding campaigns for plays are most successful with funding goals under $5,000, with 73% of all campaigns having met their funding goal. 

- What are some limitations of this dataset?

One limitation of this dataset is that there is no data for the cost of the campaigns? Do the costs vary by goal amount or duration? The costs of fundraising with Kickstarter could be an important factor. 

Are the goal and pledged amounts in US dollars? We formatted them as such; however, that there is a currency column makes me wonder if those goal and pledged amounts are already converted or not?

In creating the Theater Outcomes by Launch Date data, I looked at the data by individual years. I wondered if fund raising changes over a decade and if those early years of data were relevant. Having drilled down to just the theater category, some years had only a few campaigns, making it difficult to spot any trends.

- What are some other possible tables and/or graphs that we could create?

I would like to compare the outcomes by staff pick = TRUE or FALSE. Does being a staff pick help to have a successful campaign? 

I would also like to see a breakdown of outcomes by goal amounts by country. 