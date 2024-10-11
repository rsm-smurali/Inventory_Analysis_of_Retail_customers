Rogers Market Transaction Analysis with Amazon Just Walk Out Technology

Overview
This project analyzes transaction-level data from the Rogers Market using Amazon Just Walk Out technology on February 28, 2024. The dataset contains key columns like purchase times, session IDs, trip durations, and group sizes. The goal is to answer several business questions by applying data analytics techniques, including customer flow, inventory buildup, and verifying Little’s Law.

Key Columns
Purchase_datetime: Timestamp when a customer exits the store (considered as the purchase time).
Session_id: Identifier for groups of customers who made purchases together. Transactions with the same session ID belong to the same group.
Trip_duration_mins: Duration (in minutes) that a customer or group spends in the store.
Group_size: Number of customers who entered the store as a group and made purchases together.
Objectives
Customer Entry Analysis:

Plot the number of customers entering the store every 15 minutes from 7 AM to 11 PM.
Calculate the average number of customers per hour entering the store.
Average Flow Time:

Calculate the average trip duration per customer, considering the group size.
Determine the average time a customer spends in the store (flow time).
Inventory Build-up Diagram:

From 7 AM to 11 PM, create an inventory build-up diagram showing the number of customers inside the store over time.
Total Time & Average Inventory:

Calculate the total time spent in the store by all customers (the area under the inventory build-up diagram).
Determine the average inventory of customers in the store.
Little's Law Validation:

Use the results from the calculations above to check Little’s Law: 
𝐿 = 𝜆 × 𝑊
where:

L is the average inventory (number of customers in the store),
λ is the average arrival rate of customers,
W is the average time spent in the store (flow time).


Steps to Solve
Data Preparation:

Parse the purchase_datetime and calculate customer entry times using the formula:
entry_time = purchase_datetime −trip_duration_mins
entry_time=purchase_datetime−trip_duration_mins
Group by 15-minute intervals to plot customer entries.

Customer Flow Analysis:

For each session, calculate how long each customer spent in the store, factoring in the group size.
Compute average time per customer (flow time).
Inventory Build-up Diagram:

Track how many customers are inside the store at any given time, using entry and exit times, and plot the results.
Total Time and Average Inventory:

Compute the area under the inventory build-up diagram (total customer time).
Calculate the average number of customers inside the store (average inventory).

Validation of Little’s Law:
Using the calculated values for flow time, arrival rate, and inventory, verify Little's Law.

Tools & Technologies
Python: For data manipulation, visualization, and analysis.
pandas: To handle and manipulate time-series data efficiently.
matplotlib/seaborn: For visualizations (e.g., inventory build-up diagram).
Jupyter Notebooks: For running and documenting the analysis.
