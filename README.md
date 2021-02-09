# Tennessee_Earthquakes
EDA and Geospatial Analysis of Earthquakes in TN

## Data Question 3: Web Scraping Earthquake Data

### Part 1:
Nate Silver discusses the difficulty of predicting earthquakes in **The Signal and the Noise**. 
Nevertheless, we are trying to identify some patterns by analyzing the deadly earthquakes that have occurred since 1900.

- Read the table of earthquakes from https://en.wikipedia.org/wiki/List_of_deadly_earthquakes_since_1900 using the `requests` and/or `beautifulsoup` library and load it into df

- Data cleaning tasks included:

* Replaced empty strings with NaN
* Removed the footnotes from the 'Other Source Deaths' column
* Converted Magnitude to a numeric type. For this portion, you can ignore differences in seismic magnitude scales.
* Corrected number of deaths when there is more than one value. When there is more than one value given, choose the largest.
* Created a new column ('deaths') that evaluates the four total-death columns ('PDE Total Deaths', 'Utsu Total Deaths', 'EM-DAT Total Deaths', and 'Other Source Deaths') and populates the new column with the highest value.
* Explored the data in terms of when and where earthquakes occurred and how severe they were (magnitude, deaths, secondary effects).
- Examined factors that make earthquakes more likely and more deadly

### Part 2:
- Used the `requests` library and the USGS's API (https://earthquake.usgs.gov/fdsnws/event/1/) to retrieve information about all recorded earthquakes that occurred in Tennessee since 1900
- Examined which counties in TN are most likely to have a large earthquake and which are the least prone
- The magnittudes of TN Earthquakes seem to follow the distribution described by Nate Silver (That is, one higher magnitude is ten times less likely to occur)

![](https://github.com/savyrosea/Tennessee_Earthquakes/blob/main/pictures/Capture.PNG)

### Part 3:
- Put together findings into presentation
- It is less advisable to concentrate resources in the four major metropolitan areas (Memphis, Nashville, Chattanooga, Knoxville), instead resources should only be focused on Memphis and Knoxville areas.
- Created a plan for allocating resources that accounts for a counties likelihood to experience an earthquak, population, and population density
    
![](https://github.com/savyrosea/Tennessee_Earthquakes/blob/main/pictures/Capture2.PNG)
