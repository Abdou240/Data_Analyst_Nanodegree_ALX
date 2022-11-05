# Ford GoBike System Dataset Analysis
## by Abderrahmen Mansour


## Dataset


> The dataset contains ride data information for about 183,000 rides in the Ford GoBike system covering the greater San Francisco Bay area, with variables including user behavior (duration, date-time, station location) and demographic information (user type, gender, age)



## Key Insights for Presentation

#### Trip distribution by day of the week and hour

**On what day of the week is there the most traffic?**
> * During the weekdays, the number of trips does not differ significantly, about 27.500 trips per day.
> * At weekends, the number of trips decreases by about 50%, i.e. 14.000 trips per day.

**During which time of day is there the most traffic?**
> * The highest traffic volume occurs between 7 and 9 a.m. and between 4 and 6 p.m.
> * Between 10 a.m. and 3 p.m., the hourly traffic volume is about 7,500.
> * Before 7 a.m. and after 6 p.m., the number of trips decreases sharply.
> * During the midnight hours (1-5 a.m.), only a few people ride GoBike.


#### Durations by day of the week per user type

**What is the usage behavior of the different user types?**
> * Subscriber usage time during the week does not change much on average.
> * On weekends, the duration of customers are higher than on weekdays.
> * On average, the duration of customers is higher than that of daily subscribers.


#### Number of customers vs. Number of subscribers

> * There are 9 times more subscribers than customers in the dataset.


#### Distance Cycled/Age/Trip Duration  vs. type of Customer

> * Subscribers tend to make short trips, while customers tend to make long trips.
> * There is no significant correlation between age and customer type.
> * Subscribers tend to travel for shorter durations, while customers tend to travel for longer durations.


#### Age vs Trip Duration/Distance by different Customer types

> * Subscribers are more likely to travel between 500 and 1500 m for 4 to 8 minutes and are between 25 and 35 years old
> * Customers are more likely to travel between 1000 and 2000 m for 4 to 16 minutes and are between 25 and 35 years old

## Summary of Findings


**Univariate Exploration:**

1- The dataset contains only trips starting in February.

2- Bicycles are used more frequently during the week than on weekends.

3- Nearly 75 % of the users are male.

5 - There are 9 times more Subscribers than Customers in the dataset.

5 - The most of the trips are between 0.5 and 1.5 km. 

6 - The most common age groups are between 23 and 28 and between 30 and 35 years old.

7- The duration distribution has a long tail. When converted to a logarithmic scale, the plot can correspond to a normal distribution, with a peak between 5-20 minutes.  

8- In the `duration_min` column, there are outliers where a trip takes longer than 67.5 minutes, less than 0.05% of the Users. I therefore drop these outliers. 

9- The distribution of ages has a long tail and is left-skewed. After using a logarithmic transformation, there is a peak between 25 and 35.

10- Peaks occurred around 8 to 9 a.m. and 4 to 6 p.m., which is the same time as commuting time.


**Bivariate Exploration:**

11- The trips take longer on weekends than on weekdays.

12 - There are two peaks in the start time duration heat map, one between 8-10am and the other between 4-6pm. The duration of the two peaks are 5-10 minutes. This indicates that most users use sharing bikes for commute trips that take 5-10 minutes.

13- User type vs. duration: Subscribers on average have a shorter trips, but more outliers.

14- User type vs. sharing: Bike sharing only available for subscribers.

15- User Type vs. Day of Week: On weekdays, user type does not affect goBike's daily traffic. On weekends, the daily frequency of customers barely changes, while that of subscribers decreases sharply.

16- The 24 to 33 year-olds Users are the main group of Users, cycling for the longest duration. They spend mostly 5-10 minutes on the road. And this is the only peak value of the heatmap.

17- There are no large differences between genders regarding the duration of trips and the distance cycled.

18- Customers are more likely to ride longer distances for a longer duration, while subscribers are more likely to ride shorter distances.



**Multivariate Exploration:**

19-Subscriber usage time during the week does not change much on average, while at weekends Customer usage is slightly higher than on weekdays.


20- Most users are between 25 and 35 years old, besides there are slightly more subscribers than customers, where subscribers are more likely to travel between 500 and 1500 m for 4 to 8 minutes, while customers are more likely to travel between 1000 and 2000 m for 4 to 16 minutes, from which we can conclude that users use the service for a specific purpose, which has a specific duration of time and length.

