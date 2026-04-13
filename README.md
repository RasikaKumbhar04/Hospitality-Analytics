# 🏨 Hospitality Analytics - Project (P1194)

## Project Overview

End‑to‑end Hospitality Data Analytics using SQL, Excel, Tableau & Power BI

This project delivers a complete analytics solution for hotel performance monitoring across multiple properties and cities. It includes data cleaning, SQL modeling, dashboard development, and deep business insights derived from booking and operational data.

<img width="850" height="450" alt="Banner" src="https://github.com/user-attachments/assets/bc265442-2948-4bdf-9de7-0b2277d797e5" />


------------------------------------------------------------------------------------------------------------------

⭐ Executive Summary

This project demonstrates the full analytics lifecycle:

      ✅ Data Import → Cleaning → SQL Modeling
      ✅ Dashboard Development in Excel, Tableau, Power BI
      ✅ KPI Analysis → Booking Trends → Revenue Insights → Operational Insights
      ✅ Action‑oriented business recommendations
      
Designed as an industry‑ready BI project, this showcases strong skills across SQL, data modeling, visualization, and analytical storytelling.

------------------------------------------------------------------------------------------------------------------

⭐ Project Scope & Responsibilities

1. Data Preparation & Cleaning
   
      - Imported raw CSVs into Excel, Tableau, and MySQL
      - Cleaned null values, standardized dates, formats, and labels
      - Ensured consistent schemas across all BI tools

3. Data Relationships & Modeling
   
      Established primary relationships across:

            dim_date
            dim_hotels
            dim_rooms
            fact_bookings
            fact_aggregated_bookings

      Ensured proper joins for accurate KPI calculations and dashboard performance.

4. SQL Analysis & KPI Computation
   
   Developed SQL queries for:
      
            Revenue KPIs
            Occupancy calculations
            Demand patterns
            Cancellation & no‑show analysis
            Customer rating insights

5. Dashboard Development
   
            ✅ Excel → Pivot charts, slicers, interactive KPIs
            ✅ Tableau → Storytelling dashboards for executives
            ✅ Power BI → Live SQL connectivity, DAX measures, drill‑downs
   
      All dashboards include filters for: City, Property, Channel, Room Category, Date.

6. Business Insights & Recommendations

      - Identified top‑performing cities & properties
      - Analyzed booking channels and revenue drivers
      - Evaluated customer satisfaction trends
      - Highlighted operational inefficiencies

------------------------------------------------------------------------------------------------------------------

⭐ Tools & Technologies

      - MySQL (SQL Development)
      - Excel (Pivot-based Dashboarding)
      - Power BI (Live SQL Connection, DAX Measures)
      - Tableau (Visual Storytelling)

------------------------------------------------------------------------------------------------------------------

📁 Project Files

| Component             | File Name                                         |
|----------------------|----------------------------------------------------|
| Tableau Dashboard    | Hospitality Analysis - Tableau.twbx                |
| Excel Dashboard      | Hospitality Analytics - Excel Dashboard.xlsx       |
| Power BI Dashboard   | Hospitality Analytics - Power BI Dashboard.pbix    |
| SQL Script           | Hospitality Analytics - SQL.sql                    |
| Dataset – Dates      | dim_date.csv                                       |
| Dataset – Hotels     | dim_hotels.csv                                     |
| Dataset – Rooms      | dim_rooms.csv                                      |
| Dataset – Bookings   | fact_bookings.csv                                  |
| Dataset – Aggregated | fact_aggregated_booking.csv                        |

------------------------------------------------------------------------------------------------------------------

🗂️ Dataset Description

| Dataset Name              | Purpose                                                              |
|---------------------------|----------------------------------------------------------------------|
| dim_date                  | Provides date, month, year dimensions for analysis                   |
| dim_hotels                | Contains hotel name, property ID, and city information               |
| dim_rooms                 | Room categories and capacity details                                 |
| fact_bookings             | Detailed booking information including revenue and booking status    |
| fact_aggregated_booking   | Summary metrics such as occupancy, capacity, and successful bookings |

------------------------------------------------------------------------------------------------------------------

🧱 SQL Data Model (Star Schema)

                          dim_date
                             │
                             │  date_id = check_in_date
                             │
                ─────────────────────────────────────────
                │                                          │
                │                                          │
        fact_bookings                           fact_aggregated_bookings
                │                                          │
                │  property_id                             │  property_id
                │                                          │
             dim_hotels                                dim_hotels
                │                                          │
                │  room_category = room_id                 │  room_category = room_id
                │                                          │
             dim_rooms                                  dim_rooms

------------------------------------------------------------------------------------------------------------------

Dimension Tables

     DIM_DATE 
      - date_id    
      - full_date       
      - month       
      - year
     
     DIM_HOTELS               
       - property_id
       - property_name
       - city
     
     DIM_ROOMS
      - room_id
      - room_category
      - capacity


Fact Tables

     FACT_BOOKINGS
      - booking_id
      - property_id
      - customer_id
      - booking_date
      - check_in_date
      - checkout_date
      - room_category
      - booking_channel
      - no_guests
      - revenue_realized
      - booking_status
      - ratings_given
    
     FACT_AGGREGATED_BOOKINGS
      - date_id
      - property_id
      - room_category
      - capacity
      - successful_bookings
      - occupancy

------------------------------------------------------------------------------------------------------------------
    
🔄 Data Integration Workflow (Actual Process Used)

      - CSV Files → Excel (Dashboard)
      - CSV Files → Tableau (Dashboard)
      - CSV Files → MySQL (Import Wizard)
      - SQL Database → Power BI (Live Connection)

✅Accurate to a real-world BI workflow

✅ Minimal transformations, clean & efficient

-----------------------------------------------------------------------------------------------------------------

📊 Dashboards

✅ 1. Excel Dashboard

Interactive KPI dashboard built using Pivot Tables, charts, slicers.

📌 Includes:

    Revenue KPIs
    Occupancy trends
    Monthly performance
    Booking channel distribution
    Property-wise comparison

📁 https://drive.google.com/file/d/1Sw2JRU57IS5q2XjwUKiUnsYIJVEpHQP4/view?usp=drive_link

📸 Screenshot: https://drive.google.com/file/d/12qSPE6LaIEQMCZN_nQWh0iafnsyudKWU/view?usp=drive_link

<img width="850" height="655" alt="Excel Dashboard - HA" src="https://github.com/user-attachments/assets/f6954d80-188f-4936-8267-c416ba624835" />



✅ 2. Power BI Dashboard

Connected live with SQL for real-time updates.

📌 Includes:

    Revenue by City / Property
    Occupancy heatmaps
    Guest loyalty & ratings
    No‑show & cancellation patterns
    Drill-through pages

📁 https://drive.google.com/file/d/1l2NbdRRTLVBoMEDzBihJaxyplyzTo5Xy/view?usp=drive_link

📸 Screenshot: https://drive.google.com/file/d/1_NhXmSf2tUuh72DVzYVIvCAsd_1Cw0sr/view?usp=drive_link

<img width="850" height="671" alt="PowerBI Dashboard - HA" src="https://github.com/user-attachments/assets/5a00d8fe-19b1-47e7-87ac-f95bfba02472" />



✅ 3. Tableau Dashboard

Executive storytelling dashboard with multi-level KPIs

📌 Includes:

    Property performance
    Seasonal revenue insights
    Customer satisfaction trends
    Booking patterns

📁 https://drive.google.com/file/d/1GHtIQEqWl7acfbeyhP2swBqB1ghPgiDw/view?usp=drive_link

📸 Screenshot: https://drive.google.com/file/d/1Q-u-kkbKv_O5yl1QW0Ns8RBshbeh5SVd/view?usp=drive_link

<img width="835" height="368" alt="Tableau Dashboard - HA" src="https://github.com/user-attachments/assets/69275edc-e16e-435e-89ba-fef24da7ddc6" />


------------------------------------------------------------------------------------------------------------------

📈 Key Business Insights

 1. Revenue Insights

      - Weekdays generate the majority of revenue, contributing ₹1.06B+, driven by business travel.
      - Mumbai and top properties like Shodwe Palace contribute a large share of total revenue.
      - Elite room category drives the highest revenue due to strong demand and higher pricing.

 2. Booking Behavior Insights

      - Bookings are highest during weekdays (84,365 bookings) but occupancy is lower compared to weekends.
      - Corporate channel is the biggest driver of bookings (34,009), making it the most reliable source of demand.
      - High cancellation rate (24.83%) and missing cancellation reasons indicate operational gaps in booking data.

 3. Operational Insights

      - Weekend occupancy (73.58%) is significantly stronger than weekday occupancy (51.34%), showing better utilization on weekends.
      - No-shows (5.02%) directly impact realized revenue and daily planning.
      - Properties like Shodwe Palace outperform others, indicating varying utilization across the portfolio.


 4. Customer Insights

      - Guest feedback participation is low (77,907 ratings missing), limiting understanding of customer experience.
      - Among submitted ratings, the average score is 3.62, showing moderate satisfaction.
      - Elite rooms, being most booked, may reflect customer preference for premium amenities.

-----------------------------------------------------------------------------------------------------------------

⭐ SQL Analysis Examples

        Total Revenue
            select sum(revenue_realized) as "Total_Revenue" from Fact_bookings;
        
        Total Bookings
            select count(*) as "Total_Bookings" from fact_bookings;
      
        City wise Revenue
            Select T2.City, sum(T1.revenue_realized) as Total_Revenue from fact_bookings T1
            inner join dim_hotels T2 on T1.property_id=T2.property_id group by T2.City;

------------------------------------------------------------------------------------------------------------------

🚀 How to Run This Project

 Excel

    Open Excel file
    Click Refresh All
    Use slicers to interact

 SQL

    Import CSV files using MySQL Import Wizard
    Run Hospitality Analytics - SQL.sql
    Execute queries

 Power BI

    Open .pbix file
    Update SQL connection credentials
    Refresh dashboard

 Tableau

    Open .twbx file
    Replace CSV file paths if required
