# 🚆 Mumbai Local Train Analytics – Power BI Dashboard

## 📊 Project Overview

Mumbai Local Train Analytics is an interactive Power BI dashboard designed to analyze passenger demand, railway line performance, station traffic, popular routes, train occupancy, delays, and weather-related operational patterns.

The project transforms Mumbai local train operational data into meaningful visual insights that can help understand passenger movement and train performance across different railway lines, stations, routes, time periods, and weather conditions.

The dashboard is designed with an interactive navigation system, allowing users to move between different analytical pages and explore the data using filters and slicers.

---

## 🎯 Project Objectives

The main objectives of this project are:

- Analyze overall passenger demand across Mumbai railway lines.
- Identify high-traffic origin and destination stations.
- Identify the most popular passenger routes.
- Analyze passenger demand across different time periods.
- Compare train occupancy across train types.
- Analyze average train delays.
- Study monthly passenger demand trends.
- Examine passenger distribution across train types.
- Analyze operational patterns under different weather conditions.
- Create an interactive and user-friendly Power BI dashboard.

---

## 🛠️ Tools & Technologies

- **Power BI**
- **DAX**
- **Power Query**
- **Microsoft Excel**
- Data Modeling
- Interactive Dashboard Design

---

## 📁 Dataset

The project uses an Excel-based Mumbai local train operational dataset.

### Main data includes:

- Train operations
- Passenger counts
- Origin and destination stations
- Railway lines
- Train types
- Weather conditions
- Delay information
- Occupancy percentage
- Distance
- Estimated fare
- Date and time-period information

The dataset was modeled in Power BI using dimension and fact tables.

# 📑 Dashboard Pages

## 1️⃣ Executive Overview

This page provides a high-level overview of Mumbai local train operations.

<img width="1325" height="746" alt="Mumbai Local Train Analytics" src="https://github.com/user-attachments/assets/375a6174-705b-44b7-abcb-37e087b77a9a" />

### Key observations

- The Western Line records the highest passenger demand among the railway lines in the dataset.
- Evening Peak represents the largest share of passenger demand.
- Passenger demand varies considerably across different months.
- Average delay differs across time periods.
- Occupancy levels are relatively similar across the different train types shown.

---

## 2️⃣ Station & Route Analysis

This page focuses on station-level and route-level passenger movement.

<img width="1327" height="743" alt="Station   Route Analysis" src="https://github.com/user-attachments/assets/45201402-1bbb-49cd-bd5f-4f143af91143" />

### Key observations

- Bandra and Andheri appear among the highest passenger-origin stations in the dataset.
- Goregaon has the highest passenger volume among the displayed top destination stations.
- Slow trains account for the largest share of passengers among the displayed train types.
- Bandra → Goregaon is the highest-volume route among the displayed top routes.
- Monthly average delay changes throughout the year, with September showing a notable peak in the displayed data.

---

## 3️⃣ Weather & Operations Analysis

This page analyzes the relationship between weather conditions and train operations.

<img width="1323" height="743" alt="Wheather   Operation Analysis" src="https://github.com/user-attachments/assets/92ad94a5-d12b-4b20-837a-e7949a158dad" />

### Analysis Areas

This page helps explore:

- Passenger demand under different weather conditions.
- Average train delays associated with different weather conditions.
- Occupancy patterns under different weather conditions.
- Passenger share across weather categories.
- Changes in average delay across months and weather conditions.

> Note: The dashboard identifies patterns and associations in the dataset. It does not establish that weather directly causes delays or changes in passenger demand.

---

# 📌 Key DAX Measures

Some of the important measures used in the dashboard include:

### Total Passengers

```DAX
Total Passengers =
SUM('fact train operations'[Passengers])
