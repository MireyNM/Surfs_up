# Surfs_up
Analyse Hawaii’s weather data 
## Overview
Before opening a new surf and ice-cream shop in Hawaii, the investor, W. Avy, asked us to run some analytics on a weather data set he has from the very island where the shop will be opened. Moreover, W. Avy wants more information about temperature trends for the months of June and December. 


### Aim
The aim of this project is to perform data analysis and data exploration on a weather dataset from the island of Oahu, especially for the months of June and December, to determine if opening a surf shop is worth our time and if the surf and ice cream shop business is sustainable year-round.

## Resources 
- Data Source: hawaii.sqlite
- Software: Python 3.7.13, Jupyter Notebook, SQLite, SQLAlchemy 

## Analysis of Data and Results
Using Python, Pandas functions and methods, and SQLAlchemy, we have filtered the date column of the Measurements table in the ``` hawaii.sqlite ```  database to retrieve all the temperatures for the month of June and December respectively. <br/>
For each month, we have then converted those temperatures to a list. Finally, we have created a DataFrame from the list, and generated the summary statistics for June and December. (See Table 1 and Table 2 below ) <br/>

The code used in this step is saved as ``` SurfsUp_Challenge.ipynb``` (https://github.com/MireyNM/surfs_up/blob/main/SurfsUp_Challenge.ipynb)

<p align="center">
  <img alt="Light" src="https://user-images.githubusercontent.com/109363759/196857112-ef58d39c-4057-4eed-a96f-2acc124ca983.png" width="45%" height="45%"> 
&nbsp; &nbsp; &nbsp; &nbsp;
  <img alt="Dark" src="https://user-images.githubusercontent.com/109363759/196857148-77794773-5ed7-4145-87d4-9f5aa47eb32e.png" width="45%">
</p>

<p align="center">
Table 1: Summary statistics for June temperature
&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;
Table 2: Summary statistics for December temperature
</p>

<br/>

Table 1 and 2 shows us the following: 
- The average temperature is 71 degrees Fahrenheit in December which is slightly lower than the average temperature in June (74.94 degrees). However, the 70s are the right temperature to surf without being too cold or too hot. 
- The minimum temperature is 56 degrees in December while it is 64 degrees in June. However, 56 degrees is not considerate cold and wearing a basic wetsuit could help the surfer maintain his/her body temperature. 
- The maximum temperature is 83 degrees in December and 85 degrees in June. This shows that even in December this Island has hot days. 


## Summary 
In order to dive deeply in June and December weather we have wrote some extra queries. <br/>
(Check https://github.com/MireyNM/surfs_up/blob/main/SurfsUp_Challenge.ipynb)

**1. Summary Statistics for the station with the highest number of observations**  
In this part, we have repeated the previous work, but we have chosen data from one station only; The station that has the highest number of observations. To see if this would affect our results. (See Table 3 and 4)

<p align="center">
  <img alt="Light" src="https://user-images.githubusercontent.com/109363759/196857226-76ad4049-1d95-40eb-a85a-33cb9aa8f32f.png" width="45%"> 
&nbsp;
  <img alt="Dark" src="https://user-images.githubusercontent.com/109363759/196857251-9526045f-1a68-4279-b042-5af9e43aa696.png" width="45%">
</p>

<p align="center">
Table 3: Summary statistics for June temperature from 1 station
&nbsp; &nbsp; &nbsp;  
Table 4: Summary statistics for December temperature from 1 station
</p>

<br/>
Table 3 and 4 shows us the following: 
- The average temperature has dropped a little. It is almost 70 degrees Fahrenheit in December and 73.2 degrees in June which is still a good temperature to surf without being too cold or too hot. 
- There is not any huge difference in numbers that we should consider. We can say that these tables confirm the results of tables 1 and 2. 
- It is worth mentioning that in all tables the temperatures in the 1st quartile is in the 60s which shows that the number of days with temperatures in the 50s is low.


**2. Summary Statistics for Precipitation:** <br/>
Moreover, we have determined the summary statistics for precipitation for the months of June and December respectively (See Table 5 and 6)

<p align="center">
  <img alt="Light" src="https://user-images.githubusercontent.com/109363759/196857302-23f00c79-086d-46db-b02d-8f09e5ab4a5d.png" width="45%"> 
&nbsp; &nbsp; 
  <img alt="Dark" src="https://user-images.githubusercontent.com/109363759/196857357-605cdb6e-9153-46a2-a053-390d79e0b8ab.png" width="45%">
</p>

<p align="center">
Table 5: Summary statistics for June precipitation 
&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; 
Table 6: Summary statistics for December precipitation
</p>


In order to show the precipitation results in a different way, we have plotted a precipitation histogram for each month (See Fig.1 and 2)

<p align="center">
  <img alt="Light" src="https://user-images.githubusercontent.com/109363759/196857422-29de4a7a-f663-47e4-8c2d-c8fdc4e0fe30.png" width="45%"> 
&nbsp; &nbsp; &nbsp; &nbsp;
  <img alt="Dark" src="https://user-images.githubusercontent.com/109363759/196857590-89e8c77f-3812-4c38-a113-420e28f05a4f.png" width="45%">
</p>

<p align="center">
Fig.1: Precipitation histogram for the month of June
&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;
Fig. 2: Precipitation histogram for the month of December
</p>



- Table 5 and 6 show that the average of precipitation is 0.1 for June and 0.2 for December which is considered as light rain. <br/>
- Figures 1 and 2 shows that the precipitation level is so low in both June and December and that most of the days have a zero level of precipitation.

### Conclusion 

From this project, we can we can confirm to the investor, W. Avy, that opening a surf shop is worth our time and that the surf and ice cream shop business is sustainable year-round.
However, I would suggest to him to consider selling surf wetsuits for people who could get cold at lower temperatures (50s) and sunscreen for hot days (80s). 
