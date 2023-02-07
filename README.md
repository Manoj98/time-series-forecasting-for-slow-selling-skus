This project was done as a part of the MSA Project Week competition along with 3 other collaborators: Palash Choudhary, Sunil Ravilla, Yash Bhole

The problem statement was to forecast daily sales of slow selling SKUs for a big-box retailer. The main catch here is that slow selling SKUs (like cars) will have 
0 sales most of the days and hence, traditional time series models don't work well.

Train data available was for 5 years and had ~850K records for 575 SKUs.

After inital exploration and feature engineering, multiple techniques such as Croston, LGBM, XGB, ARIMA and Moving Average were evaluated.

The champion model utilized a novel methodology where we predicted daily sales by predicting weekly sales and also forecasting sales proportion for the day of the week for any SKU. 
The resultant daily sales would be a product of predicted weekly sales and day of the week forecasted proportion.
