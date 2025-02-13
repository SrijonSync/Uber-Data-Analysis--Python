# Uber-Data-Analysis-Python

## Overview

This project analyzes Uber ride data to uncover trends, peak hours, popular pickup locations, and other insights that can help optimize ride-sharing services. The dataset contains trip details, including timestamps, locations, and trip distances.

## Dataset

Source: The dataset was collected from Kaggle.

## Key Features:

Pickup Date & Time

Dropoff Date & Time

Pickup Location

Dropoff Location

Trip Distance

Fare Amount


## Objectives

Analyze the distribution of rides over different time periods.

Identify peak hours for Uber rides.

Discover the most popular pickup and dropoff locations.

Investigate how trip distance correlates with fare amount.

Clean and preprocess the dataset for accurate insights.

## Data Cleaning

1. Handling Missing & Duplicate Values

Checked for missing values and removed rows with crucial missing data.

Eliminated duplicate entries to maintain data integrity.

### Why this happens: Missing values could result from errors in data collection or incomplete records. Duplicates might arise due to data merging issues or multiple ride records for the same trip.

2. Formatting Date & Time Columns

Converted pickup and dropoff timestamps to proper datetime format.

Extracted hour, day, month, and day of the week from timestamps to analyze ride patterns.

### Why this happens: The original dataset may store time in string format, which is not optimal for analysis. Converting them into datetime allows better manipulation and trend identification.

3. Cleaning Location Data

Removed incorrect or inconsistent location values.

Grouped nearby locations to reduce granularity.

### Why this happens: GPS errors, user entry mistakes, or system glitches can introduce incorrect location data. Grouping locations improves accuracy in identifying key ride zones.

4. Handling Outliers

Removed trips with extremely short or long durations.

Filtered out unrealistic fare amounts and trip distances.

### Why this happens: Outliers can result from GPS errors, fraudulent activity, or data entry mistakes. Extremely low fares could indicate promotions, while unusually long trips might involve route deviations or traffic congestion.

5. Feature Engineering

Created new columns like trip duration (difference between dropoff and pickup time).

Added day of the week to analyze weekly trends.

### Why this helps: Additional features enhance analytical insights by breaking down data into meaningful categories, such as commute trends and business-hour ride patterns.

## Key Findings

1. Peak Hours for Uber Rides

Most rides occur between 7 AM - 9 AM and 5 PM - 8 PM, aligning with work commute hours.

Late-night rides increase on weekends, especially between 10 PM - 2 AM.

### Why this happens: Morning and evening rush hours see high demand as people commute to work or return home. Weekend late-night surges are influenced by nightlife and social activities.

2. Popular Pickup & Dropoff Locations

Major business districts and entertainment hubs are among the busiest pickup and dropoff points.

Airports have high ride volumes, especially during early mornings and evenings.

### Why this happens: Business areas see high demand during office hours, while entertainment hubs attract late-night traffic. Airport demand fluctuates based on flight schedules.

3. Trip Distance vs. Fare Amount

Longer trips generally have a proportional increase in fares.

Short-distance trips within city centers tend to have higher per-mile charges.

### Why this happens: Uber's fare model includes base fares, per-mile charges, and time-based fees. Short trips may appear more expensive per mile due to base fare influence.

4. Weekly Ride Distribution

Fridays and Saturdays have the highest number of trips.

Mondays have the least ride demand.

### Why this happens: Weekends encourage social activities, leading to more Uber rides. Mondays are slower due to fewer leisure activities and office workers adjusting to the workweek.

## Technologies Used

### Python

### Pandas, NumPy (for data processing)

### Matplotlib & Seaborn (for visualizations)

### Jupyter Notebook
