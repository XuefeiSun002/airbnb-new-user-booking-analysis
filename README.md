# airbnb-new-user-booking-analysis# Airbnb New User Booking Conversion Analysis

## 1. Project Overview

This project analyzes Airbnb new user booking behavior based on user profile data and web session logs.  
The main goal is to understand what factors influence whether a new user completes their first booking, identify key conversion bottlenecks, and build a predictive model to support user growth and conversion optimization.

Compared with a traditional descriptive analysis, this project focuses on four business questions:

1. Which acquisition channels bring higher-quality users?
2. Which user segments are more likely to complete their first booking?
3. Where is the major drop-off point in the user behavior funnel?
4. Can we predict users' first booking conversion tendency using profile, channel, device, and session behavior features?

---

## 2. Dataset

Data source: Kaggle Airbnb New User Bookings competition.

Main files used:

| File | Description |
|---|---|
| `train_users_2.csv` | User profile, signup information, device information, and booking destination |
| `sessions.csv` | Web session logs, including user actions, action types, devices, and time spent |
| `countries.csv` | Destination country information |
| `age_gender_bkts.csv` | Summary statistics by age, gender, and destination country |

The target variable in this project is:

```text
is_booked = 1 if country_destination != "NDF"
is_booked = 0 if country_destination == "NDF"
