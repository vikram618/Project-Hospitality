# Project-Hospitality
This repository contains my Hospitality Analytics Project
# 🏨 DA — Hospitality Analytics Project

A comprehensive end-to-end data analytics project on hospitality domain data, covering data cleaning, analysis, and visualization across **SQL**, **Excel**, **Tableau**, and **Power BI**.

---

## 📁 Project Structure

```
DA_P1171 Hospitality Analytics/
│
├── SQLFILE.sql               # Data cleaning & 38+ analytical queries
├── ExcelprojectT.xlsm        # Excel dashboard with macros
├── TABLEAUPROJECT.twbx       # Tableau workbook with interactive dashboards
└── PowerBI_Dashboard.pbix    # Power BI report (coming soon)
```

---

## 📊 Dataset Overview

The project uses a **star schema** with the following tables:

| Table | Description |
|-------|-------------|
| `fact_bookings` | Individual booking records (booking ID, dates, revenue, guests, ratings) |
| `fact_aggregated_bookings` | Aggregated bookings with capacity and successful booking counts |
| `dim_date` | Date dimension with week number and day type (weekday/weekend) |
| `dim_hotels` | Hotel master data (property name, city, category) |
| `dim_rooms` | Room dimension (room ID, room class) |

---

## 🗄️ SQL Analysis (`SQLFILE.sql`)

### Data Cleaning
- Converted string date columns to proper `DATE` format using `STR_TO_DATE()`
- Dropped and renamed columns for consistency across all fact and dimension tables

### Key Metrics Covered (38 Queries)

| # | Metric | Description |
|---|--------|-------------|
| 1 | Total Revenue | Sum of all realized revenue |
| 2 | Occupancy % | Successful bookings / Total capacity |
| 3 | Total Bookings | Count of all booking IDs |
| 4 | Total Guests | Sum of guest counts |
| 5 | Booking Status Breakdown | Checked Out / Cancelled / No Show |
| 6 | Cancellation % | Share of cancelled bookings |
| 7 | Checked Out % | Share of completed stays |
| 8 | No Show % | Share of no-show bookings |
| 9 | Utilized Capacity | Actual usage vs available capacity |
| 10–13 | Trend by Day Type & Month | Revenue and booking count by weekday/weekend and month |
| 14–15 | Hotel-wise Analysis | Booking count and revenue by property |
| 16 | City-wise Analysis | Booking and revenue by city |
| 17–18 | Category-wise Analysis | Luxury vs Business segments |
| 19–20 | Room Class Analysis | Revenue and bookings by room class |
| 21 | Booking Platform Analysis | Performance across booking channels |
| 22–23 | Average Length of Stay | Overall and hotel-wise |
| 24–25 | Average Ratings | Overall and hotel-wise guest ratings |
| 26 | Week-wise Trends | Revenue, bookings, and occupancy by week |
| 28–31 | Booking % by Platform / Class / Hotel / Day Type | Window function-based percentage share |
| 32 | ADR (Average Daily Rate) | Revenue per booking |
| 33 | Booking Status % | Distribution across statuses |
| 34 | Realisation % | Revenue realization after cancellations/no-shows |
| 35 | RevPAR | Revenue Per Available Room |
| 36 | DBRN | Daily Booked Room Nights |
| 37 | DSRN | Daily Sellable Room Nights |
| 38 | DURN | Daily Utilized Room Nights |

---

## 📗 Excel Dashboard (`ExcelprojectT.xlsm`)

- Built using **Excel with Macros (.xlsm)**
- Contains interactive dashboards with slicers and pivot tables
- Covers key hospitality KPIs: Revenue, Occupancy, ADR, RevPAR, Realisation %
- Macro-enabled for dynamic filtering and automated calculations

---

## 📈 Tableau Dashboard (`TABLEAUPROJECT.twbx`)

- Built using **Tableau Desktop**
- Packaged workbook (`.twbx`) includes embedded data
- Visualizations include:
  - Revenue and occupancy trends by week
  - City and property-wise performance
  - Booking platform contribution
  - Day type (Weekday vs Weekend) comparisons
  - Room class and category breakdowns

---

## 📊 Power BI Dashboard *(Coming Soon)*

> **Note:** The Power BI file (`PowerBI_Dashboard.pbix`) will be added to this repository shortly.

Planned visualizations:
- Executive summary with KPI cards (Revenue, Occupancy, ADR, RevPAR)
- Interactive filters by city, property, month, and room class
- Trend analysis with drill-through capabilities
- Booking platform performance matrix
- Ratings and guest experience analysis

---

## 🔑 Key Business Metrics

| Metric | Formula |
|--------|---------|
| **Occupancy %** | Successful Bookings / Total Capacity × 100 |
| **ADR** | Total Revenue / Total Bookings |
| **RevPAR** | Total Revenue / Total Available Rooms |
| **Realisation %** | 1 − (Cancellation % + No Show %) |
| **DBRN** | Total Bookings / No. of Days |
| **DSRN** | Total Capacity / No. of Days |
| **DURN** | Total Checked-Out Bookings / No. of Days |

---

## 🛠️ Tools & Technologies

| Tool | Purpose |
|------|---------|
| **MySQL** | Data storage, cleaning, and SQL analysis |
| **Microsoft Excel** | KPI dashboards with pivot tables and macros |
| **Tableau** | Interactive visual analytics |
| **Power BI** | *(Coming Soon)* Business intelligence reporting |

---

## 🚀 How to Use

1. **SQL**: Import the dataset into MySQL, run `SQLFILE.sql` sequentially — data cleaning queries first, then analysis queries.
2. **Excel**: Open `ExcelprojectT.xlsm` and enable macros when prompted.
3. **Tableau**: Open `TABLEAUPROJECT.twbx` directly in Tableau Desktop or Tableau Public.
4. **Power BI**: File will be added soon — open with Power BI Desktop once available.

---

## 👤 Author

**Vikra** — Data Analytics Project  
*Hospitality Analytics — Group 6*
