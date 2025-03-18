
# 🚖 Namma Yatri Data Analysis  

This project focuses on **extracting insights** from ride-sharing data using **SQL queries**. The analysis covers **driver performance, revenue trends, user behavior, and ride patterns**, helping to derive meaningful business intelligence from the dataset.  

## 📌 Key Insights from SQL Analysis  

### **1️⃣ Driver Performance Analysis**  
- 🔹 **Top Earning Drivers**: Identified the highest-earning drivers based on total fare earnings.  
- 🔹 **Most Active Drivers**: Ranked drivers based on the number of completed rides.  
- 🔹 **Peak Ride Hours**: Determined the busiest time slots for drivers.  

### **2️⃣ User Behavior & Demand Patterns**  
- 🔹 **Most Popular Pickup Locations**: Found the areas with the highest ride requests.  
- 🔹 **Frequent Riders**: Identified users who book the most rides.  
- 🔹 **Ride Cancellations**: Analyzed cancellation rates and common reasons.  

### **3️⃣ Revenue & Payment Insights**  
- 🔹 **Monthly Revenue Trends**: Calculated total earnings per month to track financial performance.  
- 🔹 **Pending Payments**: Identified rides with unpaid or pending transactions.  
- 🔹 **Payment Methods Used**: Analyzed the most commonly used payment methods.  

### **4️⃣ Ride Efficiency & Operations**  
- 🔹 **Average Ride Duration**: Measured the average time taken per ride.  
- 🔹 **Distance vs. Fare Analysis**: Checked whether longer rides result in proportionally higher fares.  
- 🔹 **Surge Pricing Impact**: Investigated how fare rates change during high-demand periods.  

---

## 🔍 Sample SQL Queries  

### **1️⃣ Find the Top 5 Highest Earning Drivers**  

SELECT driver_id, SUM(fare_amount) AS total_earnings  
FROM rides  
GROUP BY driver_id  
ORDER BY total_earnings DESC  
LIMIT 5;
### **2️⃣ Identify Most Popular Pickup Locations

SELECT pickup_location, COUNT(*) AS total_rides  
FROM rides  
GROUP BY pickup_location  
ORDER BY total_rides DESC  
LIMIT 10;
### **3️⃣ Retrieve Monthly Revenue Trends

SELECT DATE_FORMAT(ride_date, '%Y-%m') AS month, SUM(fare_amount) AS total_revenue  
FROM rides  
GROUP BY month  
ORDER BY month DESC;
### **4️⃣ Calculate Average Ride Duration

SELECT AVG(TIMESTAMPDIFF(MINUTE, start_time, end_time)) AS avg_ride_duration  
FROM rides;
## 🚀 How to Use This Project
### **1️⃣ Run the Queries
Open your SQL environment (MySQL, PostgreSQL, or any SQL-compatible tool).
Load the dataset if available.
Execute the provided SQL queries.
Analyze the query results for insights.
### **2️⃣ Modify for Custom Analysis
Change date ranges, locations, or filters to focus on specific data points.
Use JOINS to combine tables and extract deeper insights.
Optimize queries for faster performance.


## 🔮 Future Enhancements
🔹 Predictive Analysis – Use SQL-based trend analysis for ride demand forecasting.
🔹 Anomaly Detection – Identify fraudulent activities in ride payments.
🔹 Real-Time Analytics – Implement live tracking using SQL views.

## 📜 License
This project is open-source. Feel free to contribute, refine, or expand the SQL analysis! 🚀




