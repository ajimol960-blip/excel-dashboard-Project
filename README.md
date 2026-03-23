#  Hotel Performance Dashboard - Excel Project

## Domain: Hospitality
##  Project Overview
This project analyzes hotel booking data and presents insights through an interactive Excel dashboard.  
The dashboard includes KPIs, slicers, pivot tables, and visualizations to help understand revenue trends, guest behavior, and booking patterns.

---
##  Dataset Description
- **Domain:** Hospitality / Hotel Analytics  
- **Data Type:** Simulated hotel booking dataset  
- **Contains:**  
  - Guest information  
  - Room types  
  - Booking channels  
  - Check‑in dates  
  - Revenue  
  - Nights stayed  

> Datasets are linked by GuestID and RoomID as key columns.

---

## Steps Followed

### 1. Data Import & Cleaning (Power Query)
- Imported all 3 CSV files into Excel using Power Query
- Removed duplicate records
- Standardized date formats (CheckInDate, CheckOutDate)
- Corrected column data types
- Filtered out irrelevant/blank rows

### 2. Data Modeling (Power Pivot)
- Loaded cleaned tables into the Data Model
- Created relationships:
  - Bookings[GuestID] → Guests[GuestID]
  - Bookings[RoomID] → Rooms[RoomID]

### 3. DAX Measures Created
- **Total Revenue (AED)**
- **Total Reservations** 
- **Avg Revenue per Booking**
- **Room Nights Sold** 
- **Avg Length of Stay** 
- **Avg Daily Rate (ADR)** 

### 4. Dashboard Features
Dashboard Creation
- Designed an interactive dashboard with:
  - KPI cards  
  - Slicers (Room Type, Booking Channel, Month, Country)  
  - Bar charts, line charts, and pie charts  
  - Clean layout and consistent formatting  

## Key Performance Indicators (KPIs)
- **Total Revenue (AED):** Total money earned from bookings  
- **Total Bookings:** Number of reservations  
- **Avg Booking Value:** Average revenue per booking  
- **Total Room Nights:** Total nights stayed by guests  
- **Avg Stay Days:** Average length of stay  
- **Revenue per Night:** Revenue earned per occupied night  

## How to View the Dashboard
1. Open Hospitality_Dashboard.xlsx
2. Navigate to the **Dashboard** sheet
3. Use the **slicers** on the left and right side to filter:
   - By Room Type
   - By Booking Channel
   - By Month
   - By Country
4. All charts and KPIs update automatically

---

## Repository Contents
- Hospitality_Dashboard.xlsx - Main Excel workbook
- `Bookings.csv` - Raw bookings data
- `Guests.csv` - Guest information
- `Rooms.csv` - Room details
-  screenshot  - dashboard
- `README.md` - Project documentation

---

##  Created By: Ajimol Shaheer
               https://github.com/ajimol960-blip/excel-dashboard-Project.git

