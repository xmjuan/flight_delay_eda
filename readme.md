# Flights delay EDA
## by Ximin Juan


## Dataset

> In this dataset, there are 29 columns dated back to 2007 and capture flights operated by carries and their delays/cancellations. This dataset consists of date, depature and arrival info of airlines, flight profile (such as operating carrier, flight num), delay/cancellation and their causes. <br>
> The main causes provided above for flight delay is one of the 5 - carrier, extreme weather, nas, security and previous late aircraft, for flight cancellation there are 4, impact of delay is measured in minutes. Additionally, delay is categorized into arrival delay and depature delay.<br>
> Apart from information above, actual/CRS elapsed time, taxiing time are also provided. Some data such as AirTime and Distance are highly correlated and implying similar factors, therefore due to data size and target, some columns will not be used in this analysis.

## Data wrangling
> As the dataset is too big, leading an extremely slow process, a random sample which is 10% of the data is selected without replacing. Apart from that, a couple columns such as elapsed time have been dropped at the beginning so as to focus on main features.
> Duplicates (27 rows) are removed from the dataset. <br>
> Scheduled time have been grouped into 'morning, afternoon, evening and night'. <br>
> In the end, all columns are ajusted into proper data type.

## Data analyzing
> Followed Udacity data visualization, data analyzing process is split into unvariate exploration, bivariate exploration and multivariate exploration. <br>
> In unvariate exploration, distribution of each variables have been plotted. <br>
> In bivariate exploration, the focus is on relationship between numeric and categorical variables as well as their impact on target features - arrival delay and departure delay. <br>
> In multivariate exploration, focus is only 2 measures (delay rate and average delay time), each categorical variable is zoomed in.


## Summary of Findings

> After whole data analyzing process, some questions such as the main cause of delay and cancellation have been found. The fact that flights departing at a certain time range has the most delays is also identified and so on. 


## Key Insights for Presentation

> Take away: <br>
- In 2007, 27.8% of flights are delayed, late aircraft delay is the biggest reason.
- 2.15% of flights are cancelled, carrier control is the biggest reason.
- Carrier delay is more related to arrival delay; Weather delay/security delay/late aircraft delay is equally related to both arrival delay and departure delay; NASDelay is more related to arrival delay.
- Summer turn to have higher delay rate, in terms of weekday, Thursday and Friday have 
higher delay rate; In terms of time range, afternoon and evening turn to have higher delay rate.

## Reference:
The main coding reference is code demonstrated in Udacity Data Analyst Nano degree.