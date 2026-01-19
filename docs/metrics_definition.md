# Metric Definitions – Hospitality Revenue Analytics

This document defines the key performance metrics used in the AtliQ Grands revenue analytics dashboard. All metrics follow standard hospitality industry definitions and are designed to support revenue management decision-making.

---

## 💰 Revenue
**Definition:**  
Total realized revenue generated from completed bookings.

**Calculation:**  
Revenue = Sum of `revenue_realized`

**Business Insight:**  
Represents actual income earned, excluding cancellations and no-shows.

---

## 🏨 DSRN (Daily Sellable Room Nights)
**Definition:**  
Total number of rooms available for sale on a given day.

**Calculation:**  
DSRN = Daily room capacity  
(Excludes out-of-order or unavailable rooms)

---

## 🛏️ URN (Utilized Room Nights)
**Definition:**  
Number of rooms actually occupied by guests per day.

**Calculation:**  
URN = Successful bookings

---

## 📅 SRN (Sellable Room Nights)
**Definition:**  
Total sellable room nights for a given period (typically a month).

**Calculation:**  
SRN = Average DSRN × Number of days in the period

---

## 📊 Occupancy %
**Definition:**  
Percentage of available rooms that were occupied.

**Calculation:**  
Occupancy % = URN / DSRN

**Business Insight:**  
Indicates demand strength and capacity utilization.

---

## 💵 ADR (Average Daily Rate)
**Definition:**  
Average revenue earned per occupied room.

**Calculation:**  
ADR = Revenue / URN

**Business Insight:**  
Measures pricing effectiveness independent of occupancy.

---

## 📈 RevPAR (Revenue Per Available Room)
**Definition:**  
Revenue generated per available room.

**Calculation:**  
RevPAR = Revenue / DSRN  
or  
RevPAR = ADR × Occupancy %

**Business Insight:**  
A key hospitality KPI combining demand and pricing performance.

---

## 🧾 BRN (Booked Room Nights)
**Definition:**  
Total rooms booked per day, regardless of outcome.

**Calculation:**  
BRN = URN + Cancelled bookings + No-shows

---

## ✅ Realisation %
**Definition:**  
Percentage of booked rooms that resulted in actual stays.

**Calculation:**  
Realisation % = URN / BRN

**Business Insight:**  
Lower realization indicates higher cancellations or no-shows.

---

## 🔁 Week-on-Week (WoW) % Change
**Definition:**  
Percentage change in a metric compared to the previous week.

**Calculation:**  
WoW % = (Current Week / Previous Week) − 1

**Business Insight:**  
Highlights short-term performance momentum and volatility.

---

## 🗓️ Weekday vs Weekend
**Definition:**  
- Weekend = Friday and Saturday  
- Weekday = Sunday to Thursday

**Business Insight:**  
Used to distinguish between business-driven and leisure-driven demand patterns.

