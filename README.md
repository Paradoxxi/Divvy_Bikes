# Divvy Bikes Usage Trends: A Q2 2021 Analysis

## I. Introduction
This report examines usage patterns of Divvy Bikes, a public bike-sharing system in Chicago, during the second
quarter of 2021 (April 1–June 30). The goal of this analysis is to understand trends in bike type preferences, user
behaviour, and ride patterns across different customer segments (members and casual users). Insights from this
analysis can inform strategies for optimizing bike availability, improving customer experience, and identifying
potential growth opportunities for Divvy Bikes. The data was processed and analysed using MySQL with the
help of Navicat for data extraction and cleaning and Power BI for data visualization and reporting.

## II. Data
The dataset analysed contains over 1,000,000 records of bike rentals during the second quarter of 2021. Each
record includes details such as Ride ID, membership status (member or casual user), bike type and ride start and
end times. Key bike types include classic bikes, electric bikes, and docked bikes. The data provides a
comprehensive view of customer behaviour, covering trends in bike rental frequency, peak usage times, and
rental durations, offering valuable insights into customer retention and bike popularity over the three-month
period.

## III. Analysis
### 3.1 Bike Type Preferences
Over the three-month period, classic bikes were the most popular, accounting for 58.55% of all rides, followed
by electric bikes (34.23%) and docked bikes (7.22%). Both classic and electric bikes saw a roughly equal
distribution of usage between members (55%) and casual riders (45%). However, docked bikes were used
exclusively by casual users, totalling 75,740 rides during the quarter.

![](https://github.com/Paradoxxi/Raphael_Portfolio/blob/2166d01e61ff48fab3df4f92e95b2f202a213eb5/Screenshot%202024-12-26%20140949.png)

Fig. 1. Pie chart showing the distribution of bike usage by type. This chart illustrates the proportion of classic, electric, and docked bikes used during the observed period.

### 3.2 Usage Trends Over Time
Bike usage remained relatively stable throughout April and May, averaging 7,792 rentals per day by members
and 6,451 rentals per day by casual users. However, starting June 1, a significant decline was observed, with
average daily usage dropping to 3,172 for members and 2,818 for casual users. Peak usage days during the
period include May 1, 2, 16, 22, and 30, primarily driven by increased activity from casual riders. Members
showed smaller increases on these peak days, indicating a stronger influence of casual riders on usage spikes.

![](https://github.com/Paradoxxi/Raphael_Portfolio/blob/36c7e73ae5bdb70a9cc8315b3eab874958d91297/Screenshot%202024-12-26%20141040.png)

Fig. 2. Line chart showing the number of bike rentals from April to June. This chart tracks the daily rental count over the three-month period, highlighting trends and fluctuations in usage.

### 3.3 Hourly Usage Patterns
Member usage peaked during traditional commuting hours, particularly between 7:00–9:00 AM and 5:00–7:00
PM, aligning with the morning and evening rush hours. A continuous but lower-level usage rate of around 500
rentals per minute was sustained throughout the day. Casual riders followed a different pattern, with minimal
activity during the morning rush hour. Instead, their usage gradually increased, peaking at midday with similar
activity levels of 500 rentals per minute.

![](https://github.com/Paradoxxi/Raphael_Portfolio/blob/249034eeb7382cfc14955999e6c055c47e8fdedc/Screenshot%202024-12-26%20141025.png)

Fig. 3. Line chart showing the hourly distribution of bike rentals throughout the day. This chart illustrates the number of bike rentals at each hour, identifying peak usage times.

### 3.4 Rental Duration
Rental duration patterns revealed that most members completed rides within a short timeframe, with 80% of
rentals lasting less than 20 minutes. Casual riders tended to use bikes for longer periods, with 80% of their rides
lasting up to 40 minutes. The median rental duration peaked at 8 minutes, consistent across all user types.

Fig. 4. Line chart showing the duration of bike rides per minute. Casual rider duration peaked at over 50,000 minutes, this

which appears to be an anomaly, likely caused by bikes not being returned.

## IV. Conclusion
The analysis highlights several key trends in Divvy Bikes usage during Q2 of 2021. Classic bikes emerged as
the preferred choice among users, with a relatively equal split between members and casual riders. Electric bikes
also saw significant usage, while docked bikes were utilized exclusively by casual users. Daily rentals were
consistent through April and May, followed by a noticeable decline in June. Peaks in usage were associated with
weekends and holidays, driven primarily by casual riders.
Distinct patterns emerged between members and casual users in hourly usage and rental durations. Members
typically used bikes for shorter commutes during rush hours, while casual riders engaged in leisure trips during
midday and for longer durations.
To optimize operations, Divvy Bikes could explore strategies to address the drop in usage during June, possibly
through targeted marketing campaigns or seasonal promotions. Additionally, enhancing services for casual
riders, such as increasing bike availability near tourist destinations or introducing pricing incentives, may further
boost engagement.

### V. Appendix
Appendix A: Data Cleaning Steps The following data cleaning steps were performed:
• Fixed inaccurate data: Corrected inconsistencies in the “Start Station Name” and “Datetime Started At”
column.
• Handled missing values: Rows with missing critical data points (e.g., “End Station ID”) were removed,
while missing less important values were imputed.
Appendix B: Tools used included:
• MySQL: For data extraction, involving SQL queries to filter, aggregate and data cleaning.
• Microsoft Power BI: Used to generate insight through visuals from the dataset as seen in figure 1, 2, 3
and 4, as well as double checking the dataset with tools such as “Column Distribution” and “Column
Profile”.
• Dataset Source: Kaggle – Divvy Bikes Database
(https://www.kaggle.com/datasets/curiel/divvy-bikes-database?select=data.csv)
