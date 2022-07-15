# Introduction

![Heading](https://github.com/Mr-Art-coder/Covid19-Data-Analysis/blob/main/PANDEMIC.jpg)

Covid 19 Pandemic is a perilous disaster that ensued in China in late 2019 and shook the world from 2020 to 2021, many countries are still recovering from the impact of the virus. 
This analysis focus on the projection of the rate of the impact of the pandemic on different countries. Due to the large dataset, some visualizations were narrowed down to Top 10 and Bottom 10.

# Problem Statement

Data speaks, and it is an individual who hears what it says that can analyze the data. It is obvious that the Covid’19 pandemic shook the world, but to what extent? At what rate? was there any casualty, what was even the record? All these thoughts led to the formulation of the problem solved with the dataset gotten, the problems are adduced below.
- What are the total confirmed cases all over the world?
- How many people were lost to the virus?
- What is the totality of those that were affected but later recovered?
- Which countries were affected most?
- Which countries were least affected?
----

# Data Sourcing

The dataset used was gotten from a [CSSEGISandData GitHub Repository](https://github.com/CSSEGISandData/COVID-19/tree/master/csse_covid_19_data), it is a live data that is updated every day. Due to this, the dataset was not downloaded but it was gotten into Power BI using a web source. It was in CSV (comma-separated Version) format with 3 fact tables. 

----

# Data Transformation
![Power Query](https://github.com/Mr-Art-coder/Covid19-Data-Analysis/blob/main/Power%20Query.JPG)

As mentioned in data sourcing, the dataset contains 3 tables, each table has tons of columns and rows, and everything is identical i.e., the three tables have the same column and roles, what separates them is the table name. 
Firstly, the first row in each table was turned to the header, then the first four columns were selected in other to unpivot other columns which are just dates. After unpivoting other columns, the data was left with Province/State, Country/Region, Lat, Long, and two columns gotten after unpivoting other columns, then the two columns were named Date and Confirmed (it is named confirmed in Confirm table, death in death table and recovered in recover table).
The three tables were merged in other to have one consolidated table to work with since all the tables were identical. The merged table has six columns.
- Province/State
- Country/Region
- Lat
- Long
- Date
- Confirmed
- Death
- Recovered
In the query section, the column length of the data was removed in other for the data to refresh and fetch additional data from the source in case the dataset is updated.
A hierarchy was created for both date and country/region in other to drill down to the month, day, or drill down to region respectively.

----

# Data Analysis and Visualization
The data were analyzed using different visualization which includes the following.
- Card: To determine the total number of deaths, confirmed, and recovered cases and to also showcase the country with the high rate of confirmation cases

![Cards](https://github.com/Mr-Art-coder/Covid19-Data-Analysis/blob/main/Cards.JPG) ![Cards](https://github.com/Mr-Art-coder/Covid19-Data-Analysis/blob/main/Card%20Most%20Affected.JPG)

- Line Chart: A line chart was used to visualize the top 10 death records according to countries.
![Line Chart](https://github.com/Mr-Art-coder/Covid19-Data-Analysis/blob/main/Line%20Chart.JPG)

- Stacked Bar Chart: Used to visualize the top 10 confirmed cases according to countries.
 ![Stacked Bar Chart](https://github.com/Mr-Art-coder/Covid19-Data-Analysis/blob/main/Stacked%20Bar%20Chart.JPG)
 
- Donut Chart: To visualize the top 10 recovered cases also according to countries.
![Donut Chart](https://github.com/Mr-Art-coder/Covid19-Data-Analysis/blob/main/Donut%20Chart.JPG)

- Slicer: To filter the record according to date.

-Map: This represents the geographical representation of the location.
![Map](https://github.com/Mr-Art-coder/Covid19-Data-Analysis/blob/main/map.JPG)

----

# Findings and Recommendation
![Dashboard](https://github.com/Mr-Art-coder/Covid19-Data-Analysis/blob/main/Dashboard.JPG)

Although Covid19 erupted in China, the county is not among the top 10 affected regions, USA has the highest record of confirmed cases of over 30 million and had the highest record death rate of 456thousand.   Even though the USA is the most affected region, the region which had the highest record of recovery is India with a total number of 951 thousand out of the over 1milion affected.
Findings showcase that China where the viruses erupted was less affected because the country imposed heavy restrictions immediately in other to stop the spread of the virus. The USA is a mega country so that is the reason why it has the highest number of confirmed cases. 

----
----

Connect with me on [Twitter](https://twitter.com/Mr_Art_officia)





