#  Hotel Performance Dashboard - Excel Project

## Domain: Hospitality

---

## Dataset Description
Three related datasets were simulated for this project:

### 1. Bookings.csv
- BookingID, GuestID, RoomID, CheckInDate, CheckOutDate,
  TotalAmount, BookingChannel, BookingStatus

### 2. Guests.csv
- GuestID, GuestName, Gender, Country

### 3. Rooms.csv
- RoomID, RoomType (Deluxe/Standard/Suite),
  FloorNumber, PricePerNight

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
- **Total Revenue (AED)** = AED 532,350.00
- **Total Reservations** = 95
- **Avg Revenue per Booking** = AED 5,603.68
- **Room Nights Sold** = 279
- **Avg Length of Stay** = 3 nights
- **Avg Daily Rate (ADR)** = AED 1,908.06

### 4. Dashboard Features
####  Charts & Visuals:
- Revenue by Country (Bar Chart)
  → Top countries: USA, UK, Germany, Canada, Australia
- Monthly Revenue Trend (Line Chart)
  → Jan: 214,000 | Feb: 149,550 | Mar: 168,800
- Revenue by Channel (Donut Chart)
  → TravelAgent: 55% | Walk-in: 12% | Website: 33%
- Revenue by Room Type (Donut Chart)
  → Deluxe: 65% | Standard: 12% | Suite: 23%

####  Interactive Slicers:
- Room Type (Deluxe / Standard / Suite)
- Booking Channel (TravelAgent / Walk-in / Website)
- CheckIn Date by Month (Jan / Feb / Mar)
- Country filter

---

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
- `Hospitality_Dashboard.xlsx - Main Excel workbook
- `Bookings.csv` - Raw bookings data
- `Guests.csv` - Guest information
- `Rooms.csv` - Room details
- `README.md` - Project documentation

---

##  Name: Ajimol Shaheer
## GitHub: https://github.com/AjimolAli/hospitality-dashboard-project
