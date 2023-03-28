# SF gobike Sharing Data Exploration

## Dataset

The initial dataset consist of 183412 gobike rides with 16 variables. Here are some of them:

- Duration (seconds)
- Start time (hh:mm:ss)
- End time (hh:mm:ss)
- Start station ID
- Start station name
- End station ID
- End station name
- gobike ID
- User type (Subscriber/Customer)
- Member Gender (Male/Female/Others)
- Bike share for all trip (Yes/No)
- Member Birth Year (years)

The dataset can be found in Udacity's Communicate Data Findings - Dataset Options document, [here](https://www.google.com/url?q=https://video.udacity-data.com/topher/2020/October/5f91cf38_201902-fordgobike-tripdata/201902-fordgobike-tripdata.csv&sa=D&source=editors&ust=1679236142575389&usg=AOvVaw0nj0QuWhsT3-pR6A35VNUV), with feature documentation available [here](https://www.google.com/url?q=https://github.com/BetaNYC/Bike-Share-Data-Best-Practices/wiki/Bike-Share-Data-Systems&sa=D&source=editors&ust=1679236142576736&usg=AOvVaw1ogtCoTiWRVWb27LH85bR3).

## Summary of Findings

In exploring the duration variable, I discovered that the majority of it values were concentrated under 4000 seconds with a long tail that extends to 84000 seconds. That made it difficult to understand its distribution. Applying log transformation brought that out, but there are many extreme values that highly deviate from the mean. Upon investigation, I discovered that there were high number of trips with durations over 3600 seconds, which makes it normal.

From investigating other variables, I noticed that most trips occurred during the weekdays and at business rush hours (7-9 AM and 4-7 PM). Most of the trips were made by male who are highly likely to be subscribers with their start and end points being areas that are at the heart of San Francisco.

By plotting duration with other variables in bivariate plots, I discovered that Female and Other genders and customers take longer trips. These trips occur on weekends and users don't hardly opt for bike sharing. But the users who do opt for bike sharing are usually young. There is a higher customer proportion on weekends compared to weekdays and we have incidences of midnight cycling that take longer durations.

In the multivariate plot, I found out a relationship between duration, user gender, and user type. Also, I discovered that age and gender has an influence on bike sharing status.

## Key Insights for Presentation

My main focus is on duration and the variables from which by visualising them with duration we were able to produce meaningful insights. These variables are user type and gender.

I will start by introducing the pattern drawn from duration and user type and duration and gender. Then I will finalise by plotting the three variables together.

Also, I will include the insights from the multivariate plot of age, bike sharing, and gender. 

The presentation will end with the top ten most frquented routes. 
