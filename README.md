Uber Dashboard – Power BI Project

### Interactive Data Analytics Solution for Uber NCR Operations (India)

---

## 📋 Table of Contents
1. [Project Overview](#1-project-overview)  
2. [Data Source](#2-data-source)  
3. [Key Data Columns](#3-key-data-columns)  
4. [Data Coverage](#4-data-coverage)  
5. [Data Quality Considerations](#5-data-quality-considerations)  
6. [Dashboard Pages](#6-dashboard-pages)  
   - [Landing Page](#61-landing-page)  
   - [KPI Overview](#62-kpi-overview)  
   - [Financial Overview](#63-financial-overview)  
   - [Customer Experience Overview](#64-customer-experience-overview)  
7. [Usage Notes](#7-usage-notes)  
8. [Business Problem](#8-business-problem)  
9. [Solution Provided](#9-solution-provided)  
10. [Business Impact](#10-business-impact)  
11. [Tools & Skills Demonstrated](#11-tools--skills-demonstrated)

---

## 1. Project Overview
This **Power BI solution** provides a consolidated reporting framework for **Uber operations in the NCR region of India**.  
It integrates booking, trip, financial, and experience data into an interactive set of dashboards designed for **executives, finance teams, and operations managers**.

**Objectives:**
- Track **business performance** through reliable KPIs  
- Provide **financial insights** for decision-making  
- Monitor **customer and driver experience** to identify improvement areas  

---

## 2. Data Source
- **Table Name:** `ncr_ride_bookings`  
- **Source:** Kaggle (synthetic dataset)  
- **Granularity:** Each row represents an individual ride booking  

---

## 3. Key Data Columns

| Column Name | Description |
|--------------|-------------|
| Date | Booking date (YYYY-MM-DD) |
| Time | Booking time (HH:MM) |
| Booking ID | Unique identifier for each ride |
| Booking Status | Final status (*Completed, Cancelled, Incomplete*) |
| Customer ID | Unique rider identifier |
| Vehicle Type | Sedan, Auto, Bike, etc. |
| Pickup / Drop Location | Textual location names |
| Avg VTAT | Average time driver took to reach pickup |
| Avg CTAT | Average ride duration |
| Booking Value | Fare amount |
| Payment Method | Cash, UPI, Card, Wallet |
| Customer & Driver Ratings | Scores (1–5) |
| Cancellation Flags / Reasons | For both customer and driver |
| Incomplete Ride Reasons | Reported reasons for incomplete rides |

---

## 4. Data Coverage
- **Period:** Full year of 2024 (Jan–Dec)  
- **Geography:** National Capital Region (Delhi, Gurgaon, Noida, Ghaziabad, Faridabad, etc.)  
- **Volume:** ~150,000 records  

---

## 5. Data Quality Considerations
- Location data provided as **text only** (requires geocoding for mapping)  
- **Duplicate Booking IDs** detected — same identifier used multiple times  

---

## 6. Dashboard Pages

### 6.1 Landing Page
Provides an introduction, navigation, and context for dashboard users (Executives, Finance, Operations, Customer Experience).

### 6.2 KPI Overview
High-level executive summary including:
- Total Revenue (Sum of `Booking Value`)
- Total Bookings
- Completed Ride %
- Customer & Driver Cancellation Rates
- Average Customer Rating  
All KPIs include **Month-over-Month (MoM)** performance comparisons using custom DAX formulas.

### 6.3 Financial Overview
Focused on **revenue and payment insights**, featuring:
- Total Revenue & Average Booking Value  
- Revenue by Day & Time (Heatmap)  
- Revenue by Payment Method and Vehicle Type  
- Transaction Details Table for granular review  

### 6.4 Customer Experience Overview
Highlights **service quality metrics**:
- Ratings from both customers and drivers  
- Average ride time (CTAT) and pickup time (VTAT)  
- Cancellation reasons (by customers and drivers)  
- “No Driver Found” and incomplete ride analysis  

---

## 7. Usage Notes
> **Note:** MoM metrics may not calculate correctly when multiple months are selected simultaneously in Power BI filters.  

---

## 8. Business Problem
Uber’s NCR operations manage **thousands of rides daily**, across multiple cities, vehicle types, and payment methods.  
Key challenges included:
- Fragmented reports and **lack of visibility** for executives  
- **Limited financial tracking** for revenue analysis  
- **No consolidated view** of customer experience data  

As a result, decision-making was **slow, reactive,** and often based on **incomplete information**.

---

## 9. Solution Provided
This Power BI solution unifies booking, financial, and experience data into a **single interactive dashboard** built for three user perspectives:

1. **KPI Overview** – Real-time executive summary with MoM trends  
2. **Financial Overview** – Deep-dive into revenue, value per trip, and payment mix  
3. **Customer Experience Overview** – Insights into satisfaction, cancellations, and operational bottlenecks  

---

## 10. Business Impact
✅ Executives can make **faster, data-driven decisions**  
✅ Finance teams gain **clear visibility** into revenue streams  
✅ Operations managers can **pinpoint issues** and improve service quality  
✅ The dashboard creates a **single source of truth** across departments, reducing reporting complexity and improving alignment  

---

## 11. Tools & Skills Demonstrated
- **Power BI** – Data modelling, DAX, dashboard design  
- **SQL** – Data cleaning and transformation  
- **Python** – Data preprocessing (Pandas)  
- **Data Visualization & Storytelling** – KPI structure, user-oriented design  

---

### 🧭 How to Use
1. Download the `.pbix` file from this repository  
2. Open it using **Power BI Desktop**  
3. Explore each dashboard page using filters and slicers  
4. Review DAX measures included in the “Model” view for KPI calculations  

---

**Author:** Klaudia Rapa
📧 klaudia.rapa@outlook.com
📂 www.linkedin.com/in/klaudia-rapa
