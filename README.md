# Airline-Analysis-Project
project - data analysis - airline analysis and develop visualization dashboard using excel, power pivot, power query

# About Project
| Content | Description |
| --- | --- |
|Title               | Analysis of Airline Data|
|Name                | Kyi Thin Nu  |
|Tools               | Excel, Power Pivot and Power Query |
|Total Working Hours |16 Hours |
|Timeline            |22/Jun/2024 - 20/July/2024  |

## Objective
### Purpose: 
•	To explore the airline data nature and how the analysis could be done based on the airline data to offer insights into functioning and efficiency of the aviation industry.
### Motivation: 
•	To understand the analysis process for the specific dataset (airline dataset in this project) using Excel and Power Pivot.

## Data Source 
•	Dataset downloaded from Kaggle: https://www.kaggle.com/datasets/iamsouravbanerjee/airline-dataset/data.
•	This is a Secondary Dataset.

## Data Cleaning Process
1.	Check the data types: Are the features identified with correct data types?
2.	Check the null values.
3.	Remove the columns that are not necessary in this analysis project.  
    - Remove Customer First and Last Name
4.	Add the age group according to the age columns:  
Here are the rules for defining the age group in this project:  

|Age|Age Group|
| --- | --- |
|0-2|	Infant|
|3-12|	Child|
|13-20|	AdultJunior|
|21-35|	Adult|
|36-60|	AdultSenior|
|61-90|	Senior|
|Above 90|	GoldenAge|

5.	For Data modelling: I need to add a new sheet that contains country and airport code (country + code) // skip in this project
6.	Data Cleaning >> the arrival airport = (0, -) values
7.	Create a new column >> Route by combining Departure Airport and Arrival Airport (done)
8.	Create a new column >> Flights by combining Route and Departure Date (done)

## Dashboard Functionality
1.	Overview Session (Key Metric and KPIs)
    - Total Passengers: Display the total number of unique passengers.
    - Total Flight
        -  Merge (airport country code + arrival airport + departure status) >> total (unique flights)
2.	Passenger Demographic Analysis
    - Gender Distribution: What is the percentage of Men and Women distribution?
    - Age group distribution for airline: Which age groups are the most popular in the airline?
    - Nationality Distribution: Top 10 nationalities among the passengers.
3.	Flight Routes Analysis: Analysis of flights by departure and arrival airports.
    - The most popular routes in the airline for the year 2022? (top 10 most departure and visited country)
        - The most popular route with time series: in which month which route is popular?
    - Popular Arrival Airports
        - Which continent is the most visited?
    - Popular Departure Airports
        - the most common departure airports
    - how many routes for each day? (extra)
    - total passengers in each single flight

4.	Flight Status Analysis: What is the flight status throughout the year?
    - Flight Status Overview: Pie chart showing the distribution of flight statuses (on-time, delayed, cancelled).
        - Filter with time (Monthly, Quarterly)
        - Which month is the most happening for each flight status?
    - Flight Status by Pilot: Performance of flights categorized by pilot names (on-time, delayed, cancelled).
    - To get the pilot column back from the dataset
    - Flight Status by Airport (Airport Performance): Which airport is the most on time, delayed, cancelled?
5.	Trend Analysis
    - Flights Over Time: Line chart showing the number of flights over the months of 2022.
    - Passenger Trends Over Time: Line chart showing the number of passengers over the months of 2022.
6.	Geographical Analysis
    - Flight Routes Map: Interactive map showing flight routes from departure to arrival airports.
    - Passenger Nationality Map: Map showing the distribution of passenger nationalities.

# Metrics and Charts
1.	Overview Session (Key metrics and KPI)

|Chart Title|	Total Passengers|
| --- | --- |
|Chart Type|	Card|
|Dimensions|	Number of unique passengers|
|Metrics|	unique passengers count|


|Chart Title|	Total Flight|
| --- | --- |
|Chart Type|	Card|
|Dimensions|	Number of unique flight count|
|Metrics|	unique flight count (1 unique route = by taking a unique data from airport name, departure date, arrival airport)|  


2. Passenger Demographic Analysis

|Chart Title|	Gender Distribution|
| --- | --- |
|Chart Type|	Bar Chart / Pie Chart|
|Dimensions|	Gender (Male, Female)|
|Metrics|	Count the number of PassengerID (by Genger)|  


|Chart Title|	Age Group Distribution|
| --- | --- |
|Chart Type|	Bar Chart / Pie Chart|
|Dimensions|	Age Groups|
|Metrics|	Count the number of PassengersID (by Age Groups)|


|Chart Title|	Nationalities Distribution|
| --- | --- |
|Chart Type|	Bar Chart / Pie Chart|
|Dimensions|	Nationality|
|Metrics|	The number of passengers by Nationality|

3. Flight Route Analysis

|Chart Title	|Popular Routes|
| --- | --- |
|Chart Type|	Bar Chart|
|Dimensions|	Route|
|Metrics|	The top 10 routes (based on frequence or count)|

|Chart Title|	Popular Arrival Airports|
| --- | --- |
|Chart Type|	Bar Chart|
|Dimensions|	Arrival Airports|
|Metrics|	The most common arrival airports (based on frequence or count)|

|Chart Title|	Popular Departure Airports |
| --- | --- |
|Chart Type|	Bar Chart|
|Dimensions|	Departure Airports|
|Metrics| The most common departure airports (based on frequence or count)|

4. Flight Status Analysis

|Chart Title|	Flight Status Overview|
| --- | --- |
|Chart Type|	Pie Chart|
|Dimensions|	Flight status (on-time, delayed, cancelled)|
|Metrics|	Distribution of flight status (on-time, delayed, cancelled)|

|Chart Title|	Flight Status by Pilots|
| --- | --- |
|Chart Type|	Stacked Bar Chart|
|Dimensions|	Pilot, Flight status (on-time, delayed, cancelled)|
|Metrics|	Performance of flights categorized by pilot names (on-time, delayed, cancelled).|

Chart Title	|Flight Status by Airport (Airport Performance)|
| --- | --- |
|Chart Type|	Stacked Bar Chart|
|Dimensions|	Airport, Flight status (on-time, delayed, cancelled)|
|Metrics|	Performance of flights categorized by airport names (on-time, delayed, cancelled).|

5. Trend Analysis

| Chart Title       | Flights Over Time                    |
|-------------------|--------------------------------------|
| **Chart Type**    | Line Chart                           |
| **Dimensions**    | Number of Flights, Months            |
| **Metrics**       | The number of flights over the months of 2022 |

| Chart Title       | Routes Trends Over Time                      |
|-------------------|----------------------------------------------|
| **Chart Type**    | Line Chart                                   |
| **Dimensions**    | Number of Routes                             |
| **Metrics**       | The number of routes over the months of 2022 |

6.	Geographical Analysis

| Chart Title       | Flight Routes Map                                    |
|-------------------|-----------------------------------------------------|
| **Chart Type**    | Interactive Map                                     |
| **Dimensions**    | Departure and Arrival Airports                      |
| **Metrics**       | Flight routes from departure to arrival airports     |


| Chart Title       | Passenger Nationality Map                            |
|-------------------|-----------------------------------------------------|
| **Chart Type**    | Interactive Map                                     |
| **Dimensions**    | Nationalities                                       |
| **Metrics**       | The distribution of passenger nationalities         |

## Dashboard Mockup

<img src="./images/1. airline analysis dashboard sketch_img.png" alt="Airline Analysis Dashboard Sketch" />

## Final Report
Note: Some data are irrelevant to construct the analysis, therefore the final report is a little bit different.  

<img src="./images/2. airlie analysis final dashboard (kyi).jpg" alt="Airline Analysis Final Dashboard" />

## References
- https://github.com/shwezin-coder/Analysis-Project-Planning-Template
- Search Vizzes | Tableau Public
- https://public.tableau.com/app/profile/andy.kriebel/viz/AirlineDelays_2/AirlineDelays
- https://public.tableau.com/app/profile/madhu.samudrala/viz/Airline_14/AirlineDelaySummary
