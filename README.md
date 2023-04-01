# Video Game Sales Analysis
### Using video game sales data from 1980 to 2016 and working on Excel to gather and clean data and Excel pivot tables to create an interactive dashboard.
This report will introduce how I gather, clean, and visualise data in detail and give my business insights based on the provided data. Furthermore, I will follow the six steps of the data analysis process: ask, prepare, process, share, analyse, and act, which I learned from the Google Data Analytical Course.


# Overview
This analysis aims to discover the trend of game sales worldwide by different regions, genres, and platforms from 1980 to 2016.

## Step 1: Ask

In this process, we need to ask effective questions, define the problem, use structured thinking, and communicate with others to thoroughly understand the business context and the need of my stakeholders.

In real life, a manager might give the analyst some problems and needs that must be solved beforehand. As a result, I imagine some of the problems and needs they might provide. They required me to create an interactive dashboard to show the trend of game sales worldwide by different regions, genres, and platforms from 1980 to 2016.

Below are the requirements of the dashboard:

* 1. The dashboard must let users choose a specific year, region, platform, and genre to compare sales trends.

* 2. The dashboard must contain the top 5 game genres by sales in descending order corresponding to a chosen year, region, or platform.

* 3. The dashboard must contain the top 5 platforms by sales in descending order corresponding to a chosen year, region, or genre.

* 4. The dashboard must contain the percentage of the sales of game genres and platforms corresponding to a chosen year and region.

Below are the questions we need to answer after creating the dashboard:

* 1. Which market has the highest video game sales from 1980 to 2016?

* 2. What are the total sales of the top 5 game genres and top 5 platforms worldwide from 1980 to 2016?

* 3. What are the top 5 game genres in different regions from 1980 to 2016?

* 4. Analyse the total sales trend worldwide from 1980 to 2016 and determine what happened during the specific period.

## Step 2: Prepare

In this process, we must understand how data is generated and collected. The dataset is from Kaggle, containing a list of video games with sales of over 100,000 copies. A scrape of vgchartz.com generated it. There is only one file and one worksheet for this dataset. After downloading it, I opened the file and created a duplicate worksheet to avoid messing up the original worksheet. I will be working on the duplicate worksheet as the primary analysis worksheet.

Below is the description of the field:

· Rank — Ranking of overall sales

· Name — The games name

· Platform — Platform of the games release (i.e. PC, PS4, etc.)

· Year — Year of the game’s release

· Genre — Genre of the game

· Publisher — Publisher of the game

· NA_Sales — Sales in North America (in millions)

· EU_Sales — Sales in Europe (in millions)

· JP_Sales — Sales in Japan (in millions)

· Other_Sales — Sales in the rest of the world (in millions)

· Global_Sales — Total worldwide sales.

The worksheet looks like this. If you keep scrolling down, you can see the remaining rows.


## Step 3: Process

In this process, we will use Excel to clean up the data and maintain data integrity. Here are the steps I used to clean up data and ensure data integrity.

1. Opened the duplicate worksheet on excel and named it as Working Sheet.

2. Created a table on Working Sheet. Then, we removed duplicates, and luckily, we found no duplicates.

3. Used sort and filters to maintain data consistency and ensure no blank and cell with N/A. We found 271 rows without release year, only one and two games in 2017 and 2020, respectively. Those data will impact data integrity and need to be removed since we need to create a dashboard related to the year, and the data in 2017 and 2020 cannot be represented for the whole year.

## Step 4: Analyse

In this process, I need to collect the data I need for analysis, format and adjust data to make it easier to work with. Thus, I need to think about the elements of the dashboard we would like to create. To begin with, I would like to insert slicers to filter regions, platforms, and genres to connect graphs to offer a user-friendly dashboard. Unluckily, the areas should be in the same column to insert a slicer to filter regions’ sales. The given dataset shows sales in different areas in different columns. As a result, we need to reorganise the dataset. To solve this problem, I created a pivot table to demonstrate total sales by years, platforms, and regions.

The pivot table looks like this:


Next, we must copy and paste them to a new worksheet named Year & Genre & Platform.

The new dataset looks like this:


If you keep scrolling down, you will see the data of the previous and following years. It shows 1991 at the top because I copied and pasted the data for 1991 first.

Secondly, I want to insert a timeline to connect different graphs for users to choose years to compare the sales trend, which I will create later. However, the Year column was formatted as General type, and to create a timeline, the data type should be Date type. To sort this problem out, I added each year’s day and month by finding, replacing, and formatting them as a Date type. For example, find 1991, then replace all of them with 01/01/1991.

The finished dataset looks like this:


Now, the dataset is ready to be visualised.

## Step 5: Share & Act


Feel free to use the interactive dashboard.
In this process, we will look at the finished dashboard and analyse the game sales based on the dashboard.

Here are the descriptions of each element in the finished dashboard:

The bar chart in the upper left corner shows the total sales in the chosen year, region, game genre and platform.
The pie chart demonstrates the percentage of the total sales in the chosen year, region, game genre and platform.
The bar chart in the middle of the dashboard illustrates the total sales of the top 5 game genres in the chosen region, year, and platform.
The bar chart in the upper right corner shows the total sales of the top 5 game platforms in the chosen region, year, and genre.
The slicers on the left can be used to filter conditions.
The line chart shows the total sales and the sales trends from 1980 to 2016 in the chosen year, region, genre, and platform.
The below timeline can be used to filter years.
Analysis of the game sales based on the dashboard:

Which market has the highest sales of video games from 1980 to 2016?


The charts above show the total sales and the percentage in four regions from 1980 to 2016. North America was the most profitable market from 1980 to 2016. It made the most significant fraction with 4.3K million, followed by Europe, Japan, and other countries, which produced 2.4K million, 1.3K million and 790 million, respectively. Interestingly, the total sales of North America are around as many as the total of the other three variables. Furthermore, North America comprised 49% of total sales globally, followed by 27%, 14.6% and 9% for Europe, Japan, and other countries.

What are the total sales of the top 5 game genres and top 5 platforms worldwide from 1980 to 2016?


The above bar charts show the total sales of the top 5 game genres and platforms worldwide between 1980 and 2016. As we can see, the most popular game genre was Action, followed by Sports, Shooter, and Role-Playing and Platform. It is worth noting that the gaming platforms — PS2 and PS3 from Sony — occupy first and third place in the total sales of the top 5 gaming platforms list.

What are the top 5 game genres in different regions from 1980 to 2016?


Top 5 game genres worldwide: Action, Sports, Shooter, Role-Playing, and Platform.

Top 5 game genres in North America: Action, Sports, Shooter, Platform, and Misc.

Top 5 game genres in Europe: Action, Sports, Shooter, Racing, and Misc.

Top 5 game genres in Japan: Role-Playing, Action, Sports, Platform, and Misc.

Top 5 game genres in other countries: Action, Sports, Shooter, Racing, and Misc.

Notably, the top 5 game genres of Europe and Other are the same, and Japan was the only one with Role-Playing in the list. Furthermore, the Japanese were less interested in the Shooter game than other regions. Apart from Japan, the first, second, third and fifth most popular game genres were identical in all three markets.

Analyse the total sales trend worldwide from 1980 to 2016 and determine what happened during the specific period.


The line graph above illustrates the total sales worldwide from 1980 to 2016. The peak of worldwide sales happened in 2008, selling 680 million. However, after reaching the mountain, the total sales dropped rapidly and plummeted from 2015 to 2016. Compared to the entire global sales in 2015, which were 264 million, the total sales in 2016 were only 70 million, around four times lesser than in 2015.

From 1980 to 1995 there was a steady increase in total sales, while from 1995 to 1996 there was a sudden tripling of total sales. To find out the total sales in 1995 and 1996 to process a deeper analyse, we need to use the timeline to filter out other years, except for 1995 and 1996.


Japan was the biggest game market in 1995, while in 1996, North America surpassed Japan’s total sales to become the world’s largest market for game sales. In 1996, total sales in North America and Europe were more than three times larger than their total sales in 1995. Furthermore, the global game sales on the PS platform rose around three times, and the game sales on the GB platform grew twelve times from 1995 to 1996, which was an impressive growth.

# Key Takeaways:

1. North America was the most significant market from 1980 to 2016, which occupied 49.14% of total global sales.

2. The peak of worldwide sales happened in 2008, and a steady decrease happened after 2008.

3. The top 5 game genres worldwide from 1980 to 2016 were: Action, Sports, Shooter, Role-Playing, and Platform.

4. The top 5 platforms worldwide from 1980 to 2016 were: PS2, X360, PS3, Wii, and DS.
