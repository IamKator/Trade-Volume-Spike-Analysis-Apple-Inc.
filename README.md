# 📊 Trading Volume Spike Analysis: AAPL

This project explores the trading behaviour of stock for Apple Inc. it focuses mainly on Identifying significant changes in trading volume and analysing their impact on stock performance. Trends and patterns are uncovered, providing insights into market movement.

## 📂 Dataset Overview
- Source: The dataset contains historical stock trading data for Apple Inc. (AAPL). From Kaggle
- Timeframe: January 2020 – November 2024

## 💡 Key Insights

- Volume spikes typically accompany significant price volatility, reflecting heightened investor activity or market reactions.
- Price movements following volume anomalies vary—some show upward trends (e.g., January 29), while others reflect declines (e.g., February 24), indicating mixed market sentiment.
- Sustained high volume (e.g., February 26) may suggest ongoing uncertainty or stabilization after major events.

## 🛠️ Tools Used
- Python: Data analysis and visualization.
- Pandas: Data manipulation.
- Matplotlib: Plotting trends and insights.
- Seaborn: Plotting trends and insights

## 🐢 Steps
### Initial Inspection 
Using data.head(), data.info(), and data.shape, we get an overview of the data. 
- We can see the first few rows of the data, including the different columns.

<img width="386" alt="image" src="https://github.com/user-attachments/assets/e394e932-a357-4496-95aa-24f390914575" />

- data.info() reveals the data types of each column, presence of missing values (ifany)

<img width="340" alt="image" src="https://github.com/user-attachments/assets/e8d98e41-3d63-4de8-813e-ff227f1a80c5" />

- data.shape tells us the dataset contains a large number of rows (daily data) and several relevant columns for analysis.
  [Image]

### Data Preparation
- Removing Redundant Data and Renaming Columns: As seen above, there is an unnecessary header row “AAPL”. We go ahead to remove this unnecessary header row as it has no use.
- Data Type Conversion: The 'Date' column is converted to the correct datetime data type, allowing for proper time-series analysis. Other numeric columns are also converted to their appropriate numeric types, facilitating calculations and visualizations.
- Cleaned Data: The final cleaned_dataDataFrame is well-structured, with appropriate column names and data types, ready for in-depth analysis.
  
<img width="373" alt="image" src="https://github.com/user-attachments/assets/e7e55342-5a99-47e2-b315-2d74d1b906ce" />


### Data Exploration and Visualisation
This section focuses on understanding the patterns and insights within the data:
#### Price Trends:
 Plotting high, low, open, and close prices reveals the overall price movement of Apple stock over time. We can identify periods of growth, decline, and volatility.
 
<img width="452" alt="image" src="https://github.com/user-attachments/assets/70ef4698-b2c6-44bf-a360-20ebbf3aec9a" />

##### Observation
- The stock price has been on an upward trend since 2020. This reflects strong long-term growth and investor confidence in Apple's stock.
- Significant fluctuations in price levels are visible as sharp rises and declines. This period may coincide with market uncertainty, macroeconomic events, or company-specific developments.
- The lines for High, Low, Open, and Close prices closely follow each other, suggesting relatively narrow daily price ranges.

   
#### Average Closing Price: 
This analysis shows how the average closing price of Apple stock has trended over the years. 

<img width="319" alt="image" src="https://github.com/user-attachments/assets/2c92847a-4c57-4750-a39f-7d7dd9a7050f" />

##### Observation
- The average closing price showed consistent year-over-year growth
- Despite declining trading volumes, the steady price increase underscores strong investor demand and confidence in Apple’s performance.

#### Trading Volume:
Analysis of trading volume reveals interesting patterns

Volume by Year: We can see how the total volume of Apple stock traded changes ecvery year.

<img width="310" alt="image" src="https://github.com/user-attachments/assets/2136dac5-dc4f-4a29-b81f-5c889f6b489e" />

##### Observation
- 2020: Significantly higher trading volume, reaching approximately 40 billion. This suggests heightened market activity, likely due to:
  - Increased investor attention on tech stocks during lockdown periods.
- 2021-2024: Trading volume shows a consistent downward trend, suggesting Stabilization in market activity.

Volume Over Time:

<img width="335" alt="image" src="https://github.com/user-attachments/assets/52f3f459-cd04-46ea-b97b-cc8be0db0e13" />

##### Observation
- Trading volume spiked significantly in early 2020 but gradually declined thereafter.
- Isolated spikes towards the end of 2024 reflect occasional high-activity days, potentially due to major market events(New Iphone release).

Volume Outliers:
We identify and highlight days with unusually high trading volume.

<img width="373" alt="image" src="https://github.com/user-attachments/assets/7f234530-a28a-4633-a5b7-b7d6845a322a" />



<img width="323" alt="image" src="https://github.com/user-attachments/assets/7d03bfa7-47a6-4c82-8380-0d9c6a28428f" />

##### Observation
- Red dots represent high-volume outliers, primarily clustered in early 2020.
- Multiple spikes above 300 million in volume highlight extraordinary events in early 2020
- After 2020, outliers become less frequent, suggesting that abnormal trading activity subsided.
- Late 2024: Isolated outliers suggest a resurgence in market activity, possibly due to external factors like news, earnings reports, or economic events.





## Future Work
Further exploration such as Incorporating sentiment analysis from news or social media to contextualize anomalies can be done in future.

