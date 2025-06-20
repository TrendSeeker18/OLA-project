🚕 OLA Data Analyst Project
An end-to-end data analytics project simulating ride-booking data for OLA in Bengaluru. The project involves synthetic data generation, SQL analysis, and interactive Power BI dashboards to deliver actionable business insights.

🔗 Project Video Tutorial: Watch on YouTube
📁 Dashboard File: OLA DASHBOARD.pbix

📊 Project Overview
This project is a simulation of real-world data analysis scenarios in the ride-sharing industry. It demonstrates how a data analyst can extract meaningful insights from raw data and present them in an interactive dashboard using Power BI and SQL.

📁 Dataset Description
The dataset simulates one month of OLA ride data in Bengaluru, including over 1,00,000 rows with the following features:

Column	Description
Date, Time	Ride timestamp
Booking_ID	Unique 10-digit ID (e.g., CNR1234567)
Booking_Status	Success / Cancelled / Incomplete
Customer_ID	Unique customer identifier
Vehicle_Type	Auto, Mini, Prime Sedan, SUV, Bike, etc.
Pickup_Location, Drop_Location	50 dummy Bangalore areas
V_TAT, C_TAT	Time to reach vehicle & customer
Cancelled_Rides_by_Customer, Driver	Cancellations with reasons
Incomplete_Rides	Whether ride was incomplete
Booking_Value	Total fare of the ride
Payment_Method	Cash, UPI, Credit Card, etc.
Ride_Distance	Total distance of the trip
Driver_Ratings, Customer_Rating	Feedback ratings

📌 Key Constraints Implemented in Data
✅ 62% rides marked as successful

❌ Cancelled by Customer: < 7%

❌ Cancelled by Driver: < 18%

⛔ Incomplete Rides: < 6%

📈 Higher ride volume & booking values on weekends and match days

🎯 Realistic reasons for cancellations and incomplete rides

🔍 SQL Analysis (MySQL)
Key insights were derived using SQL:

Retrieve successful bookings

Average ride distance per vehicle type

Top 5 customers by ride count

Cancelled rides and reasons (customer & driver)

Revenue analysis by booking success

Rating analysis by vehicle type

✅ Views were created for each question to optimize repeat queries

sql
Copy
Edit
-- Example: Get successful bookings
CREATE VIEW Successful_Bookings AS
SELECT * FROM bookings WHERE Booking_Status = 'Success';
📈 Power BI Dashboard
📌 Dashboard Segments:
📅 Ride Volume Over Time

📊 Booking Status Breakdown

🚗 Top Vehicle Types by Distance

💰 Revenue by Payment Method

🙍‍♂️ Customer & Driver Ratings

❌ Cancellation Reasons

🔥 Insights:
Most common cancellation reason: Driver not moving toward pickup

SUV & Sedan rides have higher revenue but lower ride volume

Ride volume spikes observed on match days and weekends

Payment method distribution: UPI & Cash dominant

🛠️ Tools Used
Power BI – Visualization

MySQL – Data analysis

Excel – Data creation & transformation

ChatGPT – Prompt-based synthetic data generation
