Uber Fares Dataset Analysis - Power BI Dashboard
Project Overview
This project analyzes Uber ride fare data to uncover business insights using Python for data preparation and Power BI for visualization. The analysis focuses on fare distribution, time-based trends, and the relationship between fare and distance.

Table of Contents
Project Overview

Dataset

Tools Used

Methodology

Key Findings

Dashboard Features

How to Use

Recommendations

Future Work

Dataset
The dataset was sourced from Kaggle (Uber Fares Dataset) and contains the following key fields:

fare_amount: The fare for the ride

pickup_datetime: Timestamp of the ride

pickup_longitude/pickup_latitude: Pickup location coordinates

dropoff_longitude/dropoff_latitude: Dropoff location coordinates

passenger_count: Number of passengers

Tools Used
Python (Jupyter Notebook): For data cleaning and feature engineering

Power BI Desktop: For data modeling and visualization

Methodology
Data Understanding: Initial exploratory data analysis (EDA) to check structure, data types, and missing values.

Data Cleaning:

Removed impossible fares (negative, zero, or extremely high values).

Filtered out invalid coordinates.

Handled missing values (dropped or imputed).

Feature Engineering:

Extracted hour, day, month, and weekday from pickup_datetime.

Calculated distance metrics.

Visualization in Power BI:

Created interactive dashboards to explore fare distribution, time trends, and correlations.

Key Findings
Fare Distribution: Most rides fall within the $5–$15 range, with a right-skewed distribution and a median fare of $8–$10.

Time-Based Trends:

Peak demand occurs during morning (6–9 AM) and evening (4–7 PM) commuting hours.

Weekends, especially Fridays and Saturdays, show higher ride volumes.

Average fares rise late at night, likely due to surge pricing or longer rides.

Fare vs. Distance: Strong positive correlation, with higher variability for longer distances.

Busiest Periods: [Replace with specific month] had the highest ride volume, indicating seasonal demand variations.

Dashboard Features
The Power BI dashboard includes the following visualizations and interactive elements:

Fare Distribution: Histogram and box plot to analyze central tendency and outliers.

Time-Based Trends: Line charts for average fare by hour, ride volume by hour/day/month, and weekday vs. weekend comparisons.

Fare vs. Distance: Scatter plot to explore the relationship.

Interactive Filters: Slicers for month, weekday, and hour to customize the view.

Screenshots
![](./dash%20board.png)
Overview of the Power BI dashboard showing fare distribution and time trends.

![](./fare%20amount%20vs%20hour.png)
Scatter plot showing the correlation between fare amount and distance.

![](./tripdistance%20vs%20fare%20amount.png)
Line chart displaying average fare and ride volume by hour of the day.

How to Use
Clone the Repository:

bash
git clone https://github.com/yourusername/uber-fares-analysis.git
Open the Power BI File:

Download and install Power BI Desktop.

Open the uber_fares_dashboard.pbix file to explore the interactive dashboard.

Run the Jupyter Notebook:

Install the required Python libraries (pandas, numpy, matplotlib).

Open the data_cleaning_and_engineering.ipynb notebook to reproduce the data preparation steps.

Recommendations
Surge Pricing: Implement dynamic pricing during peak hours (6–9 AM, 4–7 PM) and weekends.

Off-Peak Promotions: Offer discounts or loyalty rewards during low-demand periods to balance ride volume.

Data Quality: Monitor outlier fares (e.g., above $50) to ensure accuracy.

External Factors: Integrate weather or event data for deeper insights into demand fluctuations.

Future Work
Incorporate additional datasets (e.g., weather, events) to enhance analysis.

Explore machine learning models to predict fare prices based on historical trends.

Expand the dashboard to include real-time data feeds for live monitoring.

