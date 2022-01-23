# Tableau Citibike Analysis

## Data Preparation

In order to analyze a full 12-months of data, I chose to download all of the files for the year 2020. I chose this 12-months in order to assess any impacts from COVID and because this dataset included more demographic data then what was available on the 2021 dataset.

After downloading the 2020 CSV files I used a Jupyter notebook and Pandas to accomplish the following tasks:
1. Format the start and stop time for each file
2. Add a new column for the month for each file
3. Combine each monthly data frame to create a 2020 dataframe
4. Calculate the distance between the start station and end station and add a new "distance" column
5. Convert the numeric "Gender" values to a string.
6. Calculate the user age and add a new "Age" column
7. Eport the final 2020 dataframe to a new CSV for use in Tableau

## Observation and Analysis

Based on the data visualizations of 2020 dataset, the following observations were noted:

 - The Trip Count graph indicates that, as expected, there are more trips during the warmer months. However, surprisingly the most active month is September. This could be due to riders preferring early Fall weather, or possible COVID could have impacted the number of rides. September volume was 12% above the next popular month of August.

 - Trip duration indicates that the longest trip duration appears to be in the month of May. This is most likely due to recreational users taking longer rides as the whether gets warmer in the Spring. It is possible that the duration of the trip decreases as the number of trips rise during the summer due to the tempartures being too warm for longer rides. The duration for September was much lower than May, possibly the high trip count in September was due to more commuters then recreational riders.

 - Trips by User Type indicates that during the Winter months the main users are Subscribers. This could possibly indicate that subscribers are using bikes for a commute vs. recreational riding. During the summer months there is a more even distribution between subscribers and customers. Customers tend to be warm weather riders.

 - Popular Start Times - Drilling down on the most popular month of September, the most popular start times are between the hours of 3PM to 9 PM. Most likely these hours are popular because they are after work. Surprisingly there are some trips with start times between 12 AM - 3 AM with long durations. This could be users biking to evening events/parties.

 - The data shows that the the majority of users are male and are in the 24 - 34 age category. There is missing data for gender with many showing as "unknown. Even if you account for the "unkown", and if they were all female (unlikely), males would still be the larger users. This indicates that the efforts to increase female users may not be effective and more efforts are needed to increase female users. Safety concerns may be one reason and should be investigated.

 - Start Stations sorted by trip count show that Grove St Path is the most popular station. There is anoter visualization that  shows the destination distance between the start and end station. Many trips result in returning to the start station so this data is not terribly enlightening. 

 - Destination map shows the distance between the start and end stations in September. Again many bikes are returned to the same station, but there are also some long distance trips. It is possible that these trips are for commuting to other areas of the city and not recreational in nature. More analysis should be done to gather data on recreational and commuter users.

 - Looking at the top 10 end station for each start station indicates that Liberty Light Rail and Newport Pkwy stations typically have bikes returned to the same station. This might indicate that there are a large number of recreational riders at these start stations and they are condusive to pleasure rides and popular with users.