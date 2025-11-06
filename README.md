Finance Data - Investor Preferences Analysis

Author: Almat Apseit
Date: 2025
Tools: Python (pandas, numpy, matplotlib, seaborn), MySQL, Jupyter Notebook



* Project Overview
  
This project analyzes investor preferences and behavior using real survey data from Kaggle (Finance Data - Nitin Datta).
It demonstrates a complete data analytics workflow - from data cleaning and SQL integration to visualization and business insights.


* Objectives

1. Identify the most popular investment avenues
2. Explore how age and gender influence investment decisions
3. Analyze motivational factors behind financial choices
4. Integrate MySQL queries into a Python-based analytics workflow


* Key Steps

1. Data Preparation - cleaning, renaming columns, handling missing values
2. SQL Integration - storing and querying data via MySQL (finance_db)
3. Exploratory Data Analysis - demographics, preferences, and patterns
4. Visualization - bar plots, pie charts, and correlation insights
5. SQL Queries - for data aggregation and trend detection


* Example SQL Queries
  
SELECT gender, COUNT(*) AS count FROM finance GROUP BY gender;
SELECT Investment_Avenues, COUNT(*) AS popularity FROM finance GROUP BY Investment_Avenues ORDER BY popularity DESC;
SELECT Investment_Avenues, AVG(age) AS avg_age FROM finance GROUP BY Investment_Avenues;



* Insights

- Mutual Funds and Fixed Deposits are top investment choices
- Males invest more in equities; females prefer safer avenues
- Main objectives: capital growth and financial security
- Younger groups show higher risk tolerance and diversification



* Recommendations

- Offer tailored products based on age and gender segments
- Emphasize financial literacy for risk-return understanding
- Promote balanced portfolios combining mutual funds and deposits



* Tech Stack
- Python 3.x - pandas, numpy, matplotlib, seaborn
- MySQL + SQLAlchemy (PyMySQL)
- Jupyter Notebook - analysis presentation



* To reproduce: download the Kaggle dataset, create the finance_db MySQL database, update connection credentials, and run the notebook cells sequentially.
