# Customer-Segmentation-Time-Series-Trend-Analysis with ARIMA MODEL
## Project Overview
This project performs customer segmentation using RFM (Recency, Frequency, Monetary) analysis combined with K-Means clustering to group FreshDirect customers based on their purchasing behavior. Additionally, it analyzes monthly purchase trends for each customer segment to uncover seasonal patterns and behavior changes over time.

## Objectives
- Segment customers into distinct groups based on their purchasing frequency, recency, and monetary value.
- Visualize and interpret the characteristics of each customer segment.
- Analyze time series trends of purchase amounts per segment to identify seasonality and business opportunities.
- Provide actionable business recommendations based on the analysis.

## Data
The dataset contains simulated transaction data for 1000 customers over one year. It includes:
- `customer_id`: Unique customer identifier
- `order_date`: Date of the purchase
- `amount`: Purchase amount in USD
-

###   Data Simulation
Generated synthetic transaction data with randomized purchase dates and amounts per customer.

###  RFM Feature Engineering
Calculated Recency (days since last purchase), Frequency (total number of purchases), and Monetary (total spending) for each customer.

###  Clustering
- Scaled RFM features using StandardScaler.
- Applied K-Means clustering to segment customers into 4 groups (chosen based on the Elbow method).

###  Cluster Analysis
- Examined statistical summaries and visualized distributions of RFM features by cluster.
- Interpreted customer behavior and labeled segments (e.g., loyal customers, at-risk customers).

###  Time Series Analysis
- Merged cluster labels with transaction data.
- Aggregated monthly purchase amounts per cluster.
- Visualized purchase trends over time by cluster.

### ARIMA MODEL
- Grouped transactional data by Segment and Month to create time series.
Checked stationarity using the Augmented Dickey-Fuller (ADF) test.
Applied differencing where needed to stabilize trends.
Fitted ARIMA models to key segments:
🟢 Loyal Customers — consistently high spending; used to forecast future purchase volume.

🟡 At-risk Customers — declining activity; used to predict continued drop or recovery.
Plotted forecasts to visualize expected trends and support retention strategy.

Key Insights:
Loyal customers are expected to maintain strong purchasing behavior — marketing should focus on loyalty rewards and upselling.
At-risk customers show signs of ongoing decline — re-engagement campaigns can be timed around predicted low-activity months.
ARIMA modeling provided quantitative foresight into customer value by segment, making marketing plans more proactive and data-driven.

### Business Recommendations
Provided marketing and retention strategies tailored for each customer segment based on insights.
## Tools & Libraries
- Python (pandas, numpy)
- scikit-learn (StandardScaler, KMeans)
- matplotlib & seaborn for visualization
- statsmodels for ADF test and ARIMA modeling 

## Insights
- Four distinct customer segments were identified, highlighting diverse purchasing patterns.
- Time series trends revealed seasonal variations unique to each segment.
- Marketing strategies can be optimized by targeting these segments accordingly.

## ARIMA MODEL
- Grouped transactional data by Segment and Month to create time series.
Checked stationarity using the Augmented Dickey-Fuller (ADF) test.
Applied differencing where needed to stabilize trends.
Fitted ARIMA models to key segments:
🟢 Loyal Customers — consistently high spending; used to forecast future purchase volume.

🟡 At-risk Customers — declining activity; used to predict continued drop or recovery.
Plotted forecasts to visualize expected trends and support retention strategy.

Key Insights:
Loyal customers are expected to maintain strong purchasing behavior — marketing should focus on loyalty rewards and upselling.
At-risk customers show signs of ongoing decline — re-engagement campaigns can be timed around predicted low-activity months.
ARIMA modeling provided quantitative foresight into customer value by segment, making marketing plans more proactive and data-driven.

---

*Created by kainat jabeen *
