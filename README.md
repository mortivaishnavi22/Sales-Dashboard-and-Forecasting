**SALES PERFORMANCE AND FORECASTING DASHBOARD USING POWER BI**


**Project Overview-**

This project is an interactive Sales Dashboard with Forecasting built using Power BI, designed to analyze historical sales data and predict future trends.

It combines data analysis, visualization, and time series forecasting to deliver actionable business insights.

**Dashboard Preview-**


1. Sales Performance Dashboard-

![Sales Performance Dashboard](https://github.com/user-attachments/assets/f4e1c3d4-4a9a-48af-bb23-c0c96d90e89d)

2. Sales Forecasting (15 Days Prediction)-

![Sales Forecasting](https://github.com/user-attachments/assets/727cf9a4-7f20-45d7-90d9-1d05ca8e4885)

**Objectives-**


1.Analyze sales and profit performance.


2.Identify top-performing states and categories.


3.Understand customer segments and payment behavior


4.Track monthly trends (YoY analysis)


5.Predict future sales using forecasting (15 days)



**Key KPIs-**


1. Total Sales: 1.57M

2. Quantity Sold: 22K

3. Average Delivery Time: 3.93 days

4. Profit: 29.7K


**Tools & Technologies Used-**


1. Power BI Desktop
   
2. Power Query Editor – Data cleaning & transformation
   
3. DAX (Data Analysis Expressions) – Calculations & measures
   
4. Data Modeling


**DAX Measures Used-**

1. Total Sales = SUM(SuperStore_Sales_Dataset[Sales])

2. Total Profit = SUM(SuperStore_Sales_Dataset[Profit])

3. Total Quantity = SUM(SuperStore_Sales_Dataset[Quantity])

4. Average Delivery = AVERAGE(SuperStore_Sales_Dataset[Delivery Days])

5. Sales Forecasting = 
    SUMMARIZE(
        'SuperStore_Sales_Dataset',
        'SuperStore_Sales_Dataset'[Order Date],
        "Total Sales", SUM(SuperStore_Sales_Dataset[Sales])
    )


   
**Key Insights-**
- West region contributes highest sales
  
- Technology category generates maximum revenue
  
- Standard shipping is the most used delivery mode

-Sales show seasonal fluctuations across months

-Forecast indicates steady growth trend in upcoming days
