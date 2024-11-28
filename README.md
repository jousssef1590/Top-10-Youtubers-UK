# Data Portfolio: Excel, SQL, Python, & Power BI - Top 10 youtupers in UK 

![Excel, SQL, Python, & Power BI](image/ESPB.png)

# Table of contents

- [Objective](#Objective)
- [Data Source](#Data-Source)
- [Stages](#Stages)
- [Design](#Design)
	- [Mockup](#Mockup)
	- [Tools](#Tools)
- [Development](#Development)
	- [Pseudocode](#Pseudocode)
	- [Data Exploration](#Data-Exploration)
	- [Data Cleaning](#Data-Cleaning)
	- [Transform the Data](#Transform-the-Data)
 	- [Create the SQL View](#Create-the-SQL-View)
- [Testing](#Testing)
  	- [Data Quality Tests](#Data-Quality-Tests)
- [Visualization](#Visualization)
  	- [Results](#Results)
   	- [DAX Measures](#DAX-Measures)
- [Analysis](#Analysis)
	- [Findings](#Findings)
	- [Validation](#Validation)
	- [Discovery](#Discovery)
- [Recommendations](#Recommendations)
	- [Potential ROI](#Potential-ROI)
	- [Potential Courses of Actions](#Potential-Courses-of-Actions)
 [Conclusion](#Conclusion)

# Objective
- What is the key pain point?

Create a dashboard to identify top UK YouTubers in 2024 for marketing campaigns.

- Key Features:
	- Metrics: Subscriber count, total views, total videos, engagement rate.
	- Filters: Search by niche, engagement, and subscriber growth.
	- Tools: Use YouTube API for data collection and tools like Tableau or Power BI for visualization.
	- Automation: Regular updates for real-time insights.
	- This dashboard will help the marketing team make data-driven decisions and efficiently choose YouTubers for campaigns.

This dashboard will help the marketing team make data-driven decisions and efficiently choose YouTubers for their campaigns.

### User story

As the Head of Marketing,
I want to use a dashboard that analyzes YouTube channel data in the UK,
so that I can identify the top-performing channels based on metrics like subscriber base and average views.

This will allow me to make more informed decisions about which YouTubers to collaborate with,
ensuring that each marketing campaign is as effective as possible.


# Data source
- What data is needed to achieve the objective?

  We need data on the top UK YouTubers in 2024 that includes their

- channel names

- total subscribers

- total views

- total videos uploaded

- Where is the data coming from? Kaggle [see here to find it](https://www.kaggle.com/datasets/bhavyadhingra00020/top-100-social-media-influencers-2024-countrywise?resource=download) as Excel file, and Youtube API to extract (subscribers, viewers) by python


# Stages
  
- Design
- Developement
- Testing
- Analysis

# Design
### Dashboard components required
- What should the dashboard contain based on the requirements provided?

To understand what it should contain, we need to figure out what questions we need the dashboard to answer:

1. Who are the top 10 YouTubers with the most subscribers?
2. Which 3 channels have uploaded the most videos?
3. Which 3 channels have the most views?
4. Which 3 channels have the highest average views per video?
5. Which 3 channels have the highest views per subscriber ratio?
6. Which 3 channels have the highest subscriber engagement rate per video uploaded?

For now, these are some of the questions we need to answer, this may change as we progress down our analysis.

### Dashboard mockup

Some of the data visuals that may be appropriate in answering our questions include:

1. Table
2. Treemap
3. Scorecards
4. Horizontal bar chart

![Dashboard mockup](image/Mockup.png)

### Tools

|Tool|Purpose                                                |
|-----------|-------------------------------------------------------|
|Excel      | Exploring the data                                    |
|Python     | API script, To Extract data from Youtube              |
|SQL Server | Cleaning, testing, and analyzing the data             |
|Power BI   | Visualizing the data via interactive dashboards       |
|GitHub     | Hosting the project documentation and version control |
|Mokkup AI  | Designing the wireframe/mockup of the dashboard       |

# Development

### Pseudocode

- What's the general approach in creating this solution from start to finish?
1. Get the data 
2. Explore the data in Excel
3. Create python script to extract data from youtube
4. Load the data into SQL Server
5. Clean the data with SQL
6. Test the data with SQL
7. Visualize the data in Power BI
8. Generate the findings based on the insights
9. Write the documentation + commentary
10. Publish the data to GitHub Pages

### Data exploration notes

This is the stage where you have a scan of what's in the data, errors, inconcsistencies, bugs, weird and corrupted characters etc

- What are your initial observations with this dataset? What's caught your attention so far?
1. There are at least 4 columns that contain the data we need for this analysis, which signals we have everything we need from the file without needing to contact the client for any more data.
2. The first column contains the channel ID with what appears to be channel IDS, which are separated by a @ symbol - we need to extract the channel names from this.
3. Some of the cells and header names are in a different language - we need to confirm if these columns are needed, and if so, we need to address them.
4. We have more data than we need, so some of these columns would need to be removed

### Data cleaning
- What do we expect the clean data to look like? (What should it contain? What contraints should we apply to it?)
  
The aim is to refine our dataset to ensure it is structured and ready for analysis.

The cleaned data should meet the following criteria and constraints:

- Only relevant columns should be retained.
- All data types should be appropriate for the contents of each column.
- No column should contain null values, indicating complete data for all records.

Below is a table outlining the constraints on our cleaned dataset:


|Property|Description|
|---|---|
| Number of Rows |100|
|Number of Columns|4|















   

