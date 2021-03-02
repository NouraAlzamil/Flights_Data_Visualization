# (Flight Data Exploration)
## by (Noura Alzamil)


## Dataset


>This dataset reports flights in the United States, including carriers, arrival and departure delays, and reasons for delays, from January 2007 to December 2007. The data set contains 7,453,215 flights with 29 variables on each flight, but we analyzed the first month's data. The dataset has been extracted from Harvard Dataverse (https://dataverse.harvard.edu/file.xhtml?persistentId=doi:10.7910/DVN/HG7NV7/2BHLWK&version=1.0) and comes originally from RITA. 
Moreover, two datasets have been merged with the flights' dataset to get the carriers' full names and airports' names. These two datasets have been extracted from ASA(http://statcomputing.org/dataexpo/2009/supplemental-data.html).  

>In the wrangling phase, we performed the following operations to clean the data:
    - remove the duplicated rows
    - drop the rows with canceled or diverted flights
    - merge the flights' dataset with carriers' dataset
    - merge the flights' dataset with airports' dataset
    - drop unused columns(duplicated merged columns or unused columns)
    - rename the merged columns(Description,iata_x, and iata_y)
    - replace the values of DayOfWeek with the actual days(1:Monday, 2:Tuesday, ...etc)
    - remove the outliers
    - remove Inc and Co from the airline name to make the charts more readable


## Summary of Findings


>
    - The first three weekdays have almost the same number of flights, which is almost 100000, while on the last two weekdays, the number of flights is almost 80000 per day. On the weekends the number of flights is between 60000 and 75000, so, there's a large difference between the number of flights on the weekdays and weekends.
    - Southwest Airlines has the largest number of flights, followed by American Airlines.
    - The Late Aircraft Delay has the longest average delay time compared to the other delay reasons. While the average delay time of the delayed arrived flights due to security is the shortest. So, we can conclude that security doesn't cause a significant impact on delays.
    - In Jan 2007, 24% of the flights experienced a delay in the arrival time, and  21.1% of the flights experienced a delay in the departure time.
    - As expected, the arrival delay and departure delay variables are strongly correlated, and the distance and air time variables are strongly correlated as well.
    - The worst two days to fly in are Sunday and Friday since they have the highest delay average, and the best two days to fly in are Saturday and Wednesday.
    - The Houghton County Memorial Airport, located in the State of Michigan, has the longest departure delay average due to weather conditions. The difference in numbers is significant compared to the other airports, the reason for that might be the location of the airport since the state of Michigan usually gets affected by weather conditions during the winter. (since only the data of Jan has been extracted)
    - Adak Airport and King Salmon Airport had the highest avg delay time due to security, even though that security didn't affect all other airports.
    - The three airports with the highest average delay time due to late aircraft are Marquette County Airport, Capital, and Central Wisconsin, which are also from the top 10 airports with the highest delay time average. So, we can conclude that late aircraft has a huge impact on the overall arrival delay time.
    - Hawaiian Airlines is the worst airline to fly on since it has the highest average arrival delay time. Most of the Hawaiian Airlines flights are delayed due to air carriers, e.g, maintenance or crew problems, aircraft cleaning, baggage loading, fueling, etc. And that can be an indicator of the airline's low performance.
    - The most effective two causes that affect the flights' arrival and cause a delay are the air carrier and late aircraft (previous flight using the same aircraft being late).
    - The worst two airports to fly in are Middle Georgia Regional Airport and Marquette County Airport. They have the longest delay time due to different causes.
    - The Middle Georgia Regional Airport and Lewiston Nez Perce County Airport got affected by weather conditions more than the other ten airports that have the longest delay time.
   




## Key Insights for Presentation

> We will focus on the worst weekday to fly in, and the worst airline and airport to fly on, in terms of departure and arrival delay.        
    - The proportion of the delayed flights:
        In Jan 2007, 24% of the flights experienced a delay in the arrival time, and  21.1% of the flights experienced a delay in the departure time.
    - The worst weekday to fly in (The day with the longest delay time):
        The worst two days to fly in are Sunday and Friday since they have the highest delay average, and the best two days to fly in are Saturday and Wednesday.
    - Number of flights for each airline:
        Southwest Airlines has the largest number of flights, followed by American Airlines.
    - Average delay time for each delay cause:
        Late Aircraft Delay has the longest average delay time compared to the other delay reasons. While the average delay time of the delayed arrived flights due to security is the shortest. So, we can conclude that security doesn't cause a significant impact on delays.
    -  The worst airline to fly on, in terms of arrival delay:
        Hawaiian Airlines is the worst airline to fly on since it has the highest average arrival delay time. Most of the Hawaiian Airlines flights are delayed due to air carriers, e.g, maintenance or crew problems, aircraft cleaning, baggage loading, fueling, etc. And that can be an indicator of the airline's low performance.
        The most effective two causes that affect the flights' arrival and cause a delay are the air carrier and late aircraft (previous flight using the same aircraft being late).  
    -  The worst airport to fly in, in terms of arrival delay:
        The worst two airports to fly in are Middle Georgia Regional Airport and Marquette County Airport. They have the longest delay time due to different causes.
        The Middle Georgia Regional Airport and Lewiston Nez Perce County Airport got affected by weather conditions more than the other ten airports that have the longest delay time.

        
     
    