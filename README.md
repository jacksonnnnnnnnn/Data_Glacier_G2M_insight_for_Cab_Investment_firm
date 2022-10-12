# G2M Cab 
XYZ is a private equity firm in US. Due to remarkable growth in the Cab Industry in last few years and multiple key players in the market, it is planning for an investment in Cab industry. 

- Objective : Provide actionable insights to help XYZ firm in identifying the right company for making investment.

The analysis has been divided into four parts: 
- Data Observation 
- Modify data’s format and forecast profit and number of trips for each cab type 
- Finding the factors that affect the profit for each cab company
- Recommendations for investment

## Data Exploration
- 60 Features( including 17 derived features)
- Timeframe of the data: 2016-01-31 to 2018-12-31
- Total data points :355,032

Assumptions:
- Outliers are in Location’s state columns after the separation of City and State.
- Profit of rides are calculated keeping other factors constant and only 
      Price_Charged and Cost_of_Trip features used to calculate profit.
- customer_data['customer_id'] = transaction_data['customer_id’]
- transaction_data['transactoin_id']= cab_data['transaction_id’]
- cab_data['city'] = city_data['city’]
- it will be easier and more efficient for me to EDA if I join these 4 tables above
- profit = Price_charged – cost of trip

## Hypothesis:
Why Yellow Cab make more profit than Pink Cab, but its cost of trip, price charged are also higher than Pink cab?
- Yellow Cab might have some luxury services for the customers
- Luxury Car burned mor fule than a normal car in a normal service
- Pink Car loosing profit might related to the bad services
- Because of pink car's low price and low cost of trip, their might offer normal services all the time, some of these normal services might serving with drivers' bad attitude, smelly car environment.
1. Higher price charged will lead to Higher service and higher profit
2. Higher Income customer will lead to  higher Profit
3. Longer distances will lead to higher profit
4. Lower loss will lead to higher Profit
5. Weather will affect profit for each company
