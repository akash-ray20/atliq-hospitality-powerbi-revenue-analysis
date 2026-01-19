# Data Folder – AtliQ Hospitality Revenue Analytics

## 📁 Overview
This folder contains the raw CSV datasets used to build the Power BI revenue analytics dashboard for the AtliQ Grands hospitality case study.

The data is provided in a structured format and follows a **star schema**, enabling efficient data modeling and accurate metric calculations in Power BI.

---

## 📊 Dataset Description

### 🔹 Dimension Tables

#### `dim_date.csv`
Contains calendar-related information used for time-based analysis.

**Key columns:**
- `date` – Calendar date
- `mmm yy` – Month-Year representation
- `week no` – Week number
- `day_type` – Weekday or Weekend (Weekend = Friday & Saturday)

---

#### `dim_hotels.csv`
Contains hotel-level master data.

**Key columns:**
- `property_id` – Unique hotel identifier
- `property_name` – Hotel name
- `category` – Luxury or Business
- `city` – City where the hotel is located

---

#### `dim_rooms.csv`
Contains room category information.

**Key columns:**
- `room_id` – Room identifier
- `room_class` – Standard, Elite, Premium, Presidential

---

### 🔹 Fact Tables

#### `fact_bookings.csv`
Transaction-level booking data capturing individual reservations.

**Key columns:**
- `booking_id`
- `property_id`
- `booking_date`
- `check_in_date`
- `checkout_date`
- `room_category`
- `booking_platform`
- `booking_status` – Checked Out, Cancelled, No Show
- `revenue_generated`
- `revenue_realized`
- `ratings_given`

---

#### `fact_aggregated_bookings.csv`
Daily aggregated room-level data used for occupancy and capacity metrics.

**Key columns:**
- `property_id`
- `check_in_date`
- `room_category`
- `successful_bookings` – Utilized Room Nights (URN)
- `capacity` – Daily Sellable Room Nights (DSRN)

---

## 🧠 Modeling Notes
- The dataset follows a **star schema** design.
- All dimension tables are connected to the fact tables using one-to-many relationships.
- Occupancy, ADR, and RevPAR metrics are derived using the aggregated fact table to ensure performance and accuracy.

---

## ⚠️ Usage Notes
- These files are intended for **analytical and educational purposes**.
- Data is assumed to be clean and does not include personally identifiable information (PII).
- The data represents a **simulated real-world hospitality scenario**.

---

## 📌 Source
This dataset is part of a hospitality revenue analytics case study inspired by real-world business problems faced by hotel chains.

