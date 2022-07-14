# Introduction

![Heading](https://github.com/Mr-Art-coder/Covid19-Data-Analysis/blob/main/PANDEMIC.jpg)

Covid 19 Pandemic is an astute disaster ensued in China in the late 2019 and shook the world in 2020 to 2021, many countries are still recovering from the impact of the virus. 
This analysis focus on the projection of the rate of the impact of the pandemic on different countries. Due to large dataset, some visualizations were narrowed down to Top 10 and Bottom 10.

# Problem Statement

Data speaks, and it is an individual who hears what it says that can analyze the data. It is obvious that Covid’19 pandemic shook the world, but to what extent? At what rate? was there any casualty, what was even the record? All these thoughts led to the formulation of the problem solved with the dataset gotten, the problems are adduced below.
- What are the total confirmed cases all over the world?
- How many people were lost to the virus?
- What is the totality of those that were affected but later recovered?
- Which countries were affected most?
- Which countries were lest affected?
----

# Data Sourcing

The dataset used was gotten from a [CSSEGISandData GitHub Repository](https://github.com/CSSEGISandData/COVID-19/tree/master/csse_covid_19_data), it is a live data which is updated every day. Due to this the dataset was not downloaded but it was gotten into Power BI using web source. It was in CSV (comma separated Version) format with 3 fact tables. 

----

# Data Transformation
![Power Query](https://github.com/Mr-Art-coder/Covid19-Data-Analysis/blob/main/Power%20Query.JPG)

As mentioned in data sourcing, the dataset contains 3 tables, each tables have tons of columns and rows, everything identical i.e., the three tables have the same column and roles, what separates them is the table name. 
Firstly, the first row in each table was turned to header, then the first four columns were selected in other to unpivot other columns which are just date. After unpivoting other columns, the data was left with Province/State, Country/Region, Lat, Long, and two columns gotten after unpivoting other columns, then the two columns were named Date and Confirmed (it is named confirmed in Confirm table, death in death table and recovered in recover table).
The three tables were merged in other to have one consolidated table to work with since all the tables were identical. The merged table have six columns.
- Province/State
- Country/Region
- Lat
- Long
- Date
- Confirmed
- Death
- Recovered
In the query section, the column length of the data was removed in other for the data to refresh and fetch additional data from the source in case the dataset is updated.
Hierarchy was created for both date and country/region in other to drill down to month, day or drill down to region respectively.

----

# Data Analysis and Visualization
The data was analyzed using different visualization which include the following.
- Card: To determine the total number death, confirmed and recovered cases and to also showcase the country with high rate of confirmation cases
![Cards](https://github.com/Mr-Art-coder/Covid19-Data-Analysis/blob/main/Cards.JPG) ![Cards](https://github.com/Mr-Art-coder/Covid19-Data-Analysis/blob/main/Cards.JPG)

- Line Chart: Line chart was used to visualize top 10 death record according to countries.
![Line Chart](https://github.com/Mr-Art-coder/Covid19-Data-Analysis/blob/main/Line%20Chart.JPG)

- Stacked Bar Chart: Used to visualize top 10 confirmed cases according to countries.
 ![Stacked Bar Chart](https://github.com/Mr-Art-coder/Covid19-Data-Analysis/blob/main/Stacked%20Bar%20Chart.JPG)
 
- Donut Chart: To visualize the top 10 recovered cases also according to countries.
![Donut Chart](https://github.com/Mr-Art-coder/Covid19-Data-Analysis/blob/main/Donut%20Chart.JPG)

- Slicer: To filter the record according to date.

----

# Findings and Recommendation
![Dashboard](https://github.com/Mr-Art-coder/Covid19-Data-Analysis/blob/main/Dashboard.JPG)

Although Covid19 erupted from China, the county is not among the top 10 affected regions, USA has the highest record of confirmed cases of 30billion and had the highest record of death rate of 454million.   Even though USA is the most affected region, the region which had the highest record of recovery is India with the total number of 5billion out of the 18billion affected.
Findings showcase that China where the viruses erupted from was less affected because the country imposed heavy restrictions immediately in other to stop the spread of the virus. USA is a mega country so that is the reason why it has the highest number of confirmed cases. If India can quickly recover from the pandemic which makes the have the highest record of recovery, then I will recommend USA to liaises with India in other to reduce the death rate in the country.
# Color
The pandemic represent danger and atrocity, so black and red was used in the report.




