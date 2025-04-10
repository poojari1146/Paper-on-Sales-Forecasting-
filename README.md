📈 Sales Forecasting for ABC Retail Store – Time Series Analysis & Business Insights<br>
A time series forecasting project for a community-driven retail business to improve sales prediction, inventory management, and strategic planning.

🏪 About ABC Store<br>
ABC Retail Store, located in Plymouth, MI, has proudly served the local communities of Redford, Livonia, and Plymouth for over 30 years. The store offers diverse products, hosts bi-weekly promotional events, and recently added a laundromat to expand its services. With growing online presence and partnerships with delivery services like DoorDash and Grubhub, ABC Store is adapting to modern retail needs.

🧩 Business Challenge<br>
The business faced several challenges:<br>
- Volatile and unpredictable monthly sales, especially around holidays.
- Uncertainty about the impact of a minor renovation done in February.
- The need to plan better inventory and staffing for peak seasons like December.
- A desire to evaluate if investing in larger renovations would pay off.

📊 Data Collection & Analysis<br>
- Source: Point-of-sale data from Nov 2019 to Oct 2023
- Target: Net Sales (after returns, discounts, deductions)
- Tools Used: Python (pandas, matplotlib), Excel

Key steps:<br>
- Cleaned and handled missing values and retained significant holiday outliers.
- Conducted seasonal decomposition to understand the data structure:
  - Trend: 42%
  - Seasonality: 24%
  - Random noise: 34%

🔮 Forecasting Methods Applied<br>
A variety of forecasting techniques were explored and compared:<br>

1️⃣ Naïve Forecast<br>
- Uses the most recent value as the next prediction
- MAPE: 8.79%
- Performs surprisingly well for stable seasonal patterns

2️⃣ Single Exponential Smoothing<br>
- Accounts for recent trends, better suited for short-term forecasts
- MAPE: 8.0%
- Limitations: Underperforms for older data

3️⃣ Holt’s Linear Trend Method<br>
- Adds trend component but lacks seasonal adjustment
- Moderate accuracy with visible residual volatility

4️⃣ Winter’s (Triple Exponential Smoothing)<br>
- Captures seasonality and trend
- Performed well, but showed limitations in extreme months
- Residuals suggested scope for more refined modeling

5️⃣ ARIMA (0,1,0)(0,1,1)[12]<br>
- Best fit for the data (seasonal component every 12 months)
- Passed stationarity tests, low error
- Forecasts: November = 11.71, December = 11.83, January = 11.65

6️⃣ Linear Regression<br>
- Showed a positive correlation between time and sales
- Slope = +16.03, indicating monthly growth
- Durbin-Watson = 1.21, suggesting some autocorrelation

📌 Key Findings<br>
- Holiday Season Sales (Nov–Dec) are consistently high, with a noticeable spike post-renovation
- February Renovation correlated with increased sales in following months
- Seasonality is strong, with spikes around July and December
- Forecasting should be an ongoing process to accommodate changing trends
- ARIMA model outperformed others with strong fit and generalizability

🧠 Business Recommendations<br>
- Staffing & Training: Prepare early for peak seasons (Dec/July) and use slow periods for employee training
- Inventory Management: Forecast demand to avoid over/understocking
- Marketing Strategy: Target Livonia, Plymouth, Redford — the store's core market
- Digital Transformation: Move laundromat operations to a digital platform for better analytics
- Advertising ROI: Use sales forecasts to evaluate campaign impact in real-time

📈 Future Work<br>
- Analyze the full impact of laundromat renovation on total store sales
- Develop forecasts for product-level demand
- Incorporate external variables like weather, promotions, or inflation
- Use customer segmentation to build personalized marketing forecasts

🔧 Tools & Techniques Used<br>
- Time Series Decomposition
- Seasonal ARIMA (SARIMA)
- Exponential Smoothing (Single, Holt, Winter’s)
- Regression Modeling
- Residual Analysis
- Python, Excel, Visualization with Matplotlib


