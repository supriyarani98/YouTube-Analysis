# 📊 YouTube Channel Analysis – Power BI Dashboard

This Power BI project analyzes global YouTube performance metrics using interactive visuals. It highlights total uploads, view patterns, subscriber engagement, and content categories through a rich dashboard experience.

---

![YouTube Dashboard](Youtube%20ss.png)

---

## 📁 Project Overview

This business intelligence dashboard helps answer key questions:
- Which YouTube channels have the most uploads?
- What are the top-performing content categories?
- How are subscribers engaging across channel types?
- What are the country-wise view trends?

The project uses **Power BI** with **SQL**, **Excel**, and **DAX** to extract, clean, calculate, and visualize insights.

---

## 🧹 Data Cleaning & Setup

- Removed missing values and inconsistent entries.
- Converted views, uploads, and subscriber columns to numeric format.
- Standardized column headers for clarity.
- Filtered out inactive or irrelevant records.
- Used **Excel** and **Power Query Editor** for data prep.

---

## 🛠️ Tools & Technologies

- **Power BI** – Visualization, dashboarding, DAX
- **SQL** – Data extraction and joining
- **Excel** – Initial data cleaning and pre-processing
- **DAX** – Calculated fields and KPIs

---

## 📈 Visual Insights & Metrics

### 🎯 KPI Cards
- **Maximum Uploads** – Displayed top uploader with over **301K uploads**.
- **Minimum View Ranks** – Visualized using card to highlight least-viewed channels.
- **Average Views (Last 30 Days)** – Created using a cleaned and aggregated column.

### 📊 Charts & Tables
- **Line Chart**: Highlighted channels with over **200K uploads** by title.
- **Bar Chart**: Total uploads segmented by content category.
- **Table Visual**: Channel type and `Viewed by Subscriber` ratio.
- **Table**: Country-wise video views for the last 30 days.

---

## 📐 Calculated Columns & Measures (DAX)

### ✅ Measure – `Total Uploads`
```DAX
Total Uploads = SUM(Uploads[UploadCount])


## ✅ Calculated Column – Viewed by Subscriber
-Viewed by Subscriber = DIVIDE(Uploads[Views], Uploads[Subscribers])


📊 Dashboard Highlights
Channel Type Performance: Comedy, Education, Entertainment, and Music dominate viewer engagement.

People & Blogs and News are top in upload volume.

India, Indonesia, and Brazil have the highest view counts.

Viewed by Subscriber helps compare engagement across different channel types.


📌 Outcome
This dashboard enables stakeholders to:

Understand which types of channels drive the most content and engagement.

Identify countries with the highest YouTube traffic.

Evaluate content strategy using the Viewed by Subscriber metric.

Visualize upload and view patterns clearly with dynamic visuals.



🚀 Get Started
To explore or use this dashboard:

Open the .pbix file in Power BI Desktop.

Connect to your own YouTube dataset (optional).

Update calculated fields as needed.

Refresh and publish the report to Power BI Service if required.
