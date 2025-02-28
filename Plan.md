Thoughts to Optimize

1. Metric
- WMSE vs. MSE optimization
- maybe feed MSE model outputs into WMSE model?

2. Potential features

Pricing
- sale price
- sale price detrended (over other items in same category)
- sale 

Day trends
- day of week effects (per item, item category)
- yearly / seasonal effects (per each item, item category)

Holidays

3. To Investigate

Calendar
- are there ever 2 events? what do snap_state mean


Plan and Setup

- need to have a robust testing framework (or I am just spamming random things, not understanding what is going on)
- XGB model
    - setup: RepeatedKFold within the train set
    - price features: ema 0.1 (or similar)
    - categorical variables
    - holidays
    

4. Short term - current ToDos

Investigate missing sell price
- how often is sell price missing, does it always mean 0 sale?
- how much missing in test

Try XGBoost with more features
- date features
- sell price, sell price z score, sell price z score / group's sell price z score for that day