# IPL Analytics Dashboard (2022–2025) 🏏📊

An end-to-end IPL Analytics Dashboard Project built using Python, Power BI, DAX, and Power Query to analyze IPL matches from 2022 to 2025 using ball-by-ball cricket data.

This project focuses on transforming raw cricket data into an interactive and analytics-driven dashboard capable of delivering insights related to:

Team performance
Player analysis
Match trends
Venue analysis
Toss impact
Batting and bowling metrics

The dashboard was designed as a portfolio project to demonstrate practical skills in:

Data Cleaning
Data Modeling
Data Visualization
Business Intelligence
Sports Analytics
Project Objectives

The main objective of this project was to:

Build a complete analytics workflow from raw dataset to interactive dashboard
Perform proper data validation and cleaning
Create analytics-ready tables using Python
Design a professional multi-page Power BI dashboard
Generate meaningful cricket insights through data storytelling
Tools & Technologies Used
Tool	Purpose
Python	Data cleaning & preprocessing
Pandas	Data manipulation
NumPy	Statistical calculations
Power BI	Dashboard creation
DAX	Measures & KPIs
Power Query	Data transformation
GitHub	Project hosting & documentation
Dataset Information
Dataset Type: IPL Ball-by-Ball Dataset
Seasons Covered: 2022–2025
Source: Kaggle IPL Dataset
Total Rows: ~70,000+ ball-by-ball records
Data Includes:
Match details
Batting statistics
Bowling statistics
Toss information
Venue details
Wicket events
Phase-wise match data
Project Workflow

The project was completed in the following stages:

1. Data Validation

Before dashboard creation, the dataset was validated to ensure:

Correct number of matches per season
Overs consistency
Venue consistency
Proper innings data
Duplicate handling
Null value inspection
Super over identification
Key Validation Checks
Maximum over validation (0–19)
Match count verification
Venue standardization
Incomplete match removal
Super over handling
2. Data Cleaning & Transformation

The raw dataset was cleaned and transformed using Python.

Cleaning Tasks Performed
Team Standardization

Example:

Delhi Daredevils → Delhi Capitals
Kings XI Punjab → Punjab Kings
Venue Cleaning

Fixed inconsistent venue naming across seasons.

Null Handling

Removed or handled:

Review-related columns
Empty power surge columns
Unnecessary null-heavy columns
Data Type Conversion
Converted date columns
Corrected numeric columns
Boolean handling for analytics
3. Analytics-Ready Tables Created

The raw dataset was transformed into multiple structured tables for Power BI analysis.

BallByBall Table

Main granular dataset where:

1 row = 1 delivery
Features Added
Match phase classification
Dot ball indicator
Boundary indicator
Legal wicket identification
Display over formatting
Used For
Phase analysis
Match trends
Batting insights
Bowling insights
MatchSummary Table

Match-level aggregated dataset where:

1 row = 1 match
Includes
Teams
Venue
Toss details
Match winner
Innings scores
Match result type
Used For
KPI cards
Venue analysis
Toss analysis
Match trends
BatterStats Table

Player-level batting analytics table.

Metrics Calculated
Runs scored
Balls faced
Strike rate
Fours & sixes
Boundary %
50s & 100s
Used For
Orange Cap analysis
Batter comparison
Aggressive batting analysis
BowlerStats Table

Player-level bowling analytics table.

Metrics Calculated
Wickets
Economy rate
Dot ball %
Bowling average
3W & 5W hauls
Used For
Purple Cap analysis
Bowling efficiency
Pressure bowling analysis
TeamPerformance Table

Team-level aggregated analytics table.

Metrics Included
Matches played
Matches won
Win percentage
Team runs
Team wickets
Boundary counts
Used For
Team comparison
Team success analysis
Overall performance metrics
Power BI Data Modeling

The project follows a structured Power BI data model with:

Fact tables
Aggregated tables
Relationship management
Relationships Used
From	To	Relationship
MatchSummary	BallByBall	One-to-Many
MatchSummary	BatterStats	One-to-Many
MatchSummary	BowlerStats	One-to-Many
Teams	TeamPerformance	One-to-Many
Dashboard Pages

The Power BI dashboard contains multiple analytical pages.

Page 1 — IPL Overview Dashboard

Provides a high-level overview of IPL analytics.

Key Features
Total Matches KPI
Total Runs KPI
Total Wickets KPI
Total Sixes KPI
Highest Team Score KPI
Runs by Season Trend
Top Batters
Top Bowlers
Toss Decision Analysis
Venue-wise Average Score
Phase-wise Runs Distribution
Page 2 — Team Performance Analysis

Focused on team-level insights and comparison.

Key Features
Team-wise Win Percentage
Matches Won Analysis
Boundary Analysis
Team Bowling Analysis
Toss Impact
Team Comparison Table
Interactive Team Slicer
Page 3 — Player Performance Analysis

Focused on batting and bowling performance.

Key Features
Orange Cap Leaders
Purple Cap Leaders
Strike Rate Analysis
Economy Rate Analysis
Boundary Percentage
Dot Ball Percentage
Scatter Plot Analytics
Key Insights Generated

Some major insights observed from the dashboard:

Death overs contribute the highest scoring rate
Batting strike rates increased significantly in recent seasons
Certain venues consistently produce higher first innings scores
Teams winning toss often prefer chasing
High dot-ball percentage bowlers usually maintain lower economy rates
Boundary percentage helps identify aggressive finishers
Key Power BI Features Used
DAX Measures

Created custom measures for:

Total Matches
Total Runs
Total Wickets
Win Percentage
Average Venue Score
Boundary Metrics
Interactive Features
Dynamic slicers
Cross-filtering
Page-level filtering
Tooltips
Conditional formatting
Dashboard Design Principles

The dashboard was designed with focus on:

Clean layout
Minimal clutter
Consistent colors
Interactive storytelling
Professional visual hierarchy
Folder Structure
IPL-Analytics-Dashboard/
│
├── data/
│   ├── raw_dataset.csv
│   ├── ball_by_ball.csv
│   ├── batter_stat.csv
│   ├── bowler_stat.csv
│   ├── match_summary.csv
│   └── team_performance.csv
│
├── dashboard/
│   ├── IPL_Dashboard.pbix
│   └── IPL_Dashboard.pdf
│
├── images/
│   ├── dashboard_overview.png
│   ├── team_analysis.png
│   └── player_analysis.png
│
├── notebooks/
│   └── data_cleaning.ipynb
│
├── README.md
│
└── requirements.txt
Future Improvements

Possible future enhancements for this project:

Live IPL API integration
Real-time dashboard updates
Predictive analytics for match outcomes
Player similarity analysis
Advanced win probability models
Streamlit/Web deployment
Learning Outcomes

This project helped strengthen my understanding of:

Data cleaning & preprocessing
Data modeling in Power BI
DAX calculations
Dashboard design
Data storytelling
Sports analytics
Interactive visualization
Screenshots

(Add your dashboard screenshots here)

Example:

![Dashboard Overview](images/dashboard_overview.png)
Project Files
Power BI Dashboard

(Add PBIX file link)

Dashboard PDF

(Add PDF link)

Dataset

(Add dataset/source link)

Connect With Me
LinkedIn

(Add your LinkedIn profile)

GitHub

(Add your GitHub profile)

Feedback

Feedback and suggestions are always welcome.
If you found this project useful or interesting, feel free to connect or share your thoughts.

⭐ If you liked this project, consider giving it a star on GitHub!
