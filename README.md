# 🚖 Namma Yatri Project 

The **Namma Yatri Project** is a structured SQL-based system designed to manage ride-sharing operations, including users, drivers, rides, and transactions. It ensures efficient ride tracking, payment processing, and analytics support.  

## 📌 Key Features  
✅ **User & Driver Management** – Stores user and driver details securely.  
✅ **Ride Tracking** – Logs ride history, fare details, and locations.  
✅ **Payment Processing** – Manages transactions and fare calculations.  
✅ **Analytics-Ready** – Optimized for reporting and business insights.  

## 🗂️ Database Schema Overview  
This database includes multiple interconnected tables:  

| Table Name | Description |  
|------------|-------------------------------------------|  
| `users` | Stores user details (name, contact, role: rider/driver) |  
| `drivers` | Contains driver-specific data |  
| `rides` | Tracks ride details (pickup, drop-off, fare, time) |  
| `payments` | Manages ride payments, statuses, and transaction logs |  

## 🚀 Setup & Installation  
### **1. Import the SQL Database**  
To import the SQL file into **MySQL**, run:  
```bash
mysql -u username -p database_name < Poject_Namma_Yatri.sql
