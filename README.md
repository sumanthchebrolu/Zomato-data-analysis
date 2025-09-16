🍽️ Zomato Data Analysis Using Python
📌 Project Overview

Food delivery and dining apps like Zomato have revolutionized the restaurant industry. With thousands of restaurants listed, understanding customer preferences, pricing strategies, and ratings is key for businesses to stay competitive.

This project performs an exploratory data analysis (EDA) on the Zomato dataset using Python. The analysis focuses on cleaning raw restaurant data, transforming features for better usability, and visualizing trends that reveal what drives customer ratings and restaurant success.

The project is beginner-friendly but covers professional data analysis steps, making it useful for both learning and real-world application.

📂 Dataset Details

File Used: Zomato.csv

Total Records: ~50,000+ restaurant entries

Geography: Multiple cities and localities

Key Attributes:

Column	Description
name	Restaurant name
online_order	Online ordering availability (Yes/No)
book_table	Table booking availability (Yes/No)
rate	Customer rating (converted to numeric)
votes	Number of customer votes
approx_cost(for two people)	Approximate cost for two people
location	Restaurant location
cuisines	Types of cuisines offered
Data Quality Issues Addressed

Ratings like "4.1/5" converted into numeric values (e.g., 4.1).

Missing values in rate, cost, and cuisines handled properly.

Inconsistent formatting in cost values standardized.

Removed duplicate and irrelevant rows for clean analysis.

🛠️ Project Workflow
1. Importing Libraries

Pandas, NumPy → Data cleaning and preprocessing

Matplotlib, Seaborn → Visualizations

import pandas as pd
import numpy as np
import matplotlib.pyplot as plt
import seaborn as sns

2. Data Preprocessing

Cleaned and standardized rate column using a custom function.

Filled missing values with appropriate replacements.

Converted cost strings to numeric values.

Created additional derived features (e.g., average rating per cuisine).

3. Exploratory Data Analysis (EDA)

Key analyses performed:

⭐ Ratings Distribution

Most restaurants have ratings between 3.0 and 4.5.

Very few restaurants are rated above 4.8.

🛵 Online Order vs. Ratings

Restaurants that allow online ordering often attract more votes and better ratings.

🍴 Table Booking Analysis

Restaurants with table booking facilities tend to have higher customer satisfaction.

🍲 Popular Cuisines

Top cuisines include North Indian, Chinese, and Continental.

Multi-cuisine restaurants perform better than single-cuisine ones.

💰 Cost vs. Rating

Higher cost restaurants don’t always guarantee higher ratings.

Many affordable restaurants receive equally good (or better) reviews.

📍 Location Insights

Certain hotspots/localities have a higher concentration of top-rated restaurants.

4. Data Visualization

Visualizations were created to support findings:

Histograms → Ratings distribution

Count Plots → Online order & table booking impact

Box Plots → Cost vs. Rating comparisons

Heatmaps → Correlation between numerical features

Bar Charts → Top cuisines and locations

These plots give actionable insights into customer behavior and restaurant strategies.

📊 Key Insights

Online delivery & table booking significantly influence customer ratings.

North Indian & Chinese cuisines dominate the market.

Customer votes correlate strongly with ratings (more reviews = more reliability).

Affordable restaurants can achieve ratings similar to expensive ones.

Restaurant location is an important factor — popular areas attract better ratings.

🚀 Technologies Used

Programming Language: Python

Libraries:

Pandas, NumPy → Data cleaning & transformation

Matplotlib, Seaborn → Visualization

🔮 Future Enhancements

Apply Machine Learning models to predict restaurant ratings based on features.

Perform sentiment analysis on textual reviews (if available).

Build a dashboard using Streamlit, Power BI, or Tableau for interactive exploration.

Add geospatial analysis to map restaurant density and performance by area.

📌 How to Run the Project

Clone the repository:

git clone https://github.com/your-username/zomato-data-analysis.git
cd zomato-data-analysis


Install dependencies:

pip install -r requirements.txt


Run the Jupyter Notebook:

jupyter notebook "Zomato Data Analysis Using Python.ipynb"


✨ This project provides a data-driven understanding of restaurant performance on Zomato and showcases the power of EDA in Python for solving real-world business problems.
