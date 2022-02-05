# bikesharing
Exploring Bike-Sharing Data with Tableau. Create Worksheets, dashboards, and stories from New York City bike-sharing data.

## Overview of Project

In this module we'll explore Tableau, a data analysis and visualization tool that is nearly ubiquitous in today's professional world. Tableau is so popular because it allows data visualization professionals to create assets that are visually appealing and easy for a non-technical audience to understand. We want to make our visualizations so clear and so helpful that they become our stakeholders go to resource when making key decisions. Tableau will help us to do this by providing us the tools to create powerful analytic dashboards that both tell a clear story and can be easly shared with others.

What if you could start a similar bike-share business for your hometown of Des Moines Iowa? We do have a potential angel investor who might be interested in providing seed funding to explore a bike-share program in Des Moines. the mechanics of making this business work might be quite different in Des Moines than in New York City. So we decide that the first step is to figure out how the bike-share business actually works in New York City, From there we'll create a proposal on how it might work in Des Moines. Using data analytics experience we can take the lead on figuring out how this project might actually work.

This assignment is related to the Bootcamp Data Analytics from the University of Toronto. It comprises the goals below for this module: 

Follow below the goals for this module:

1) Objective 1: Change Trip Duration to a Datetime Format
2) Objective 2: Create Visualizations for the Trip Analysis
3) Objective 3: Create a Story and Report for the Final Presentation


## Resources

* Data Source: [NYC Biking Sharing Project Story and Dashboard](https://public.tableau.com/app/profile/douguot/viz/NYCBikingSharingProjectStoryandDashboard/NYCCitibikeStory), [NYC_CitiBike_Challenge.ipynb](https://github.com/DougUOT/bikesharing/blob/main/NYC_CitiBike_Challenge.ipynb) and the database is available on [201908-citibike-tripdata.csv.zip](https://s3.amazonaws.com/tripdata/201908-citibike-tripdata.csv.zip)
* Software & Data Tools: Jupyter Notebook, Tableau and Visual Studio Code 1.63.2

## Results & Code

## Objective 1: Change Trip Duration to a Datetime Format

* The data in the "tripduration" column is converted to a datetime datatype and has the correct time format

![](https://github.com/DougUOT/bikesharing/blob/main/Resources/Images/Capture14_1_1.PNG)
![](https://github.com/DougUOT/bikesharing/blob/main/Resources/Images/Capture14_1_2.PNG)

* The DataFrame is exported as a new file without the index column

![](https://github.com/DougUOT/bikesharing/blob/main/Resources/Images/Capture14_1_3.PNG)

## Objective 2: Create Visualizations for the Trip Analysis

* There is a line graph displaying the number of bikes checked out by duration for all users, and the graph can be filtered by the hour

    * The graph belows shows the number of bikes check out for all users by tripduration in minutes. We considered for the analysis below the first two hours, however its possible to use the filter available on the right side. The goal of this graph is provide how many time in minutes the users use the bike for ride. As according to the results below, the majority of users tend to ride between 5 and 10 minutes, after 20 minutes, the time in minutes decreases dramatically as the hours increase in the graph below. 

![](https://github.com/DougUOT/bikesharing/blob/main/Resources/Images/Capture14_2_1.PNG)

* There is a line graph displaying the number of bikes that are checked out by duration for each gender by the hour, and the graph can be filtered by the hour and gender

    * The line graphs below shows the number of bikes checkout in two hours by gender (male, female or unknown). It is available the filter on the right side, for gender and tripduration in hours. The goal of this graph is shows how many users by gender, during the first two hours are checkout and using the bikes. As according to the results below in  the graph the male gender is the main user for using bicicle ride.

![](https://github.com/DougUOT/bikesharing/blob/main/Resources/Images/Capture14_2_2.PNG)

* A heatmap is created showing the number of bike trips for each hour of each day of the week

    * The heatmap below shows the number of bicicle rides related to each day of the week by hour. The goal of this heatmap is shows the day and time preferred by users for the bike ride. The stronger and darker the color on the heatmap, the greater the concentration and results.  As according to the results below in heatmap Thursday is the most preferred day by users, followed by Tuesday and Monday and the most busiest time, is between 5pm and 6pm. 

![](https://github.com/DougUOT/bikesharing/blob/main/Resources/Images/Capture14_2_3.PNG)

* A heatmap is created showing the number of bike trips by gender for each hour of each day of the week, and the heatmap can be filtered by gender

    * The heatmap below shows the number of bicicle rides related to each day of the week by hour and gender. The goal of this heatmap is shows the day and time preferred by gender for the bike ride. The stronger and darker the color on the heatmap, the greater the concentration and results. As according to the results below in heatmap Thursday is the most preferred day by male, followed by Tuesday and Monday and the most preferred time by male, is between 5pm and 6pm, followed by 8am.

![](https://github.com/DougUOT/bikesharing/blob/main/Resources/Images/Capture14_2_4.PNG)

* A heatmap is created showing the number of bike trips for each type of user and gender for each day of the week, and you can only filter by user and gender

    * The heatmap below shows the number of bicicle rides related to each day of the week by user type (customer and subscriber) and by gender. The purpose of this heat map is to show the day, type of user and gender that most use the bike ride during the week. The stronger and darker the color on the heatmap, the greater the concentration and results. As according to the results below in heatmap Thursday and Fridays are the most preferred day by subscriber for both gender (male and female), however males who are subscribers use more bike rides. 

![](https://github.com/DougUOT/bikesharing/blob/main/Resources/Images/Capture14_2_5.PNG)

## Objective 3: Create a Story and Report for the Final Presentation

### Overview of the statistical analysis:

* The male gender is the primary user of bicycle rides, representing 65% of the total rides. Males have 1,530,272 rides, compared to a total of 2,344,224 rides.

* Thursday is the most preferred day by users, followed by Tuesday and Monday, being the busiest time between 5:00 pm and 6:00 pm, mainly for males, who in addition to these times also use 8:00 am on these same days. In these three times, the total number of rides are 87004 rides. 

* Thursdays and Fridays are the most preferred days by subscribers for both sexes (male and female), but male subscribers use bicycle ride more. In addition, the subscriber customers represent 697433 rides on Tuesday, Thursdays and Friday.

* Most users usually cycle between 5 and 10 minutes. Most bikes are returned before 20 minutes of use.

* Young people born between 1984 and 1995 represent 1,048,244 rides or 44% of the bikes rides. On the other hand, it is crucial to consider that people born after 1969 also use the service. 

### Provide two additional visualizations:

The visualizations below were made additionally for this project. The first graph shows the number of cyclists by year of birth. The goal is to visually identify demographic information based on year of birth; this analysis can help determine target audiences or develop strategies for marketing campaigns.

The second graph analyzes users by gender and year of birth.

As a result of this analysis, considering the number of rides by gender and birth year. According to this graphic visualization, it is highlighted that the most significant number of customers is male. The majority of the customers are young people born between 1984 and 1995, representing 1,048,244 rides or 44% of the bikes rides. On the other hand, it is crucial to consider that people born after 1969 also use the service. 

![](https://github.com/DougUOT/bikesharing/blob/main/Resources/Images/Capture14_3_1.PNG)

### Suggestions for future analysis and visualization for this project 

I suggest two analyses of start and end trips to complement this project, using maps for visualization. These analyses would be helpful as they could help the company organize logistics and resources to serve customers better. For example, you could make more bikes available for top start trips locations. The main spots for bicycle returns should have a process to return or distribute the bikes for new customers at strategic points in the city. 

## Tableau Public URL (Link to Dashboard and Story):

[NYCCitibikeStory](https://public.tableau.com/app/profile/douguot/viz/NYCBikingSharingProjectStoryandDashboard/NYCCitibikeStory)

### Below are the Images published on the  Tableau Public website (see the link above).

The NYC Biking Sharing Project and Dashboard has six parts; 

### 1) Project Overview

![](https://github.com/DougUOT/bikesharing/blob/main/Resources/Images/Capture14_4_1.PNG)

### 2) Dashboard & Analysis Overview

![](https://github.com/DougUOT/bikesharing/blob/main/Resources/Images/Capture14_4_2.PNG)

### 3) Analysis per Trips on the Weekday and Checkout Times

![](https://github.com/DougUOT/bikesharing/blob/main/Resources/Images/Capture14_4_3.PNG)

### 4) Analysis per Gender & Birth Year

![](https://github.com/DougUOT/bikesharing/blob/main/Resources/Images/Capture14_4_4.PNG)

### 5) Analysis per Gender

![](https://github.com/DougUOT/bikesharing/blob/main/Resources/Images/Capture14_4_5.PNG)

### 6) Recommendations

![](https://github.com/DougUOT/bikesharing/blob/main/Resources/Images/Capture14_4_6.PNG)


## Others Informations

* Images extract from [Citibike](https://ride.citibikenyc.com/how-it-works), [citi bike logo](https://d21xlh2maitm24.cloudfront.net/nyc/Citi-Bike-provided-by-Lyft-Positive-170x57px.svg?mtime=20201023151104), [bike image citibike](https://d21xlh2maitm24.cloudfront.net/nyc/meet-the-bike.png?mtime=20160504142030) and [Des Moines Iowa](https://i.ytimg.com/vi/bCYyTk6NgKg/maxresdefault.jpg)



















