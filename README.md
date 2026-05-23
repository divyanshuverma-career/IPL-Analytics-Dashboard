# 🏏 IPL Analytics Dashboard (2022–2025)

An end-to-end **IPL Analytics Dashboard Project** built using **Python, Power BI, DAX, and Power Query** to analyze IPL matches from **2022–2025** using ball-by-ball cricket data.

This project focuses on transforming raw cricket data into an interactive and analytics-driven dashboard capable of delivering insights related to:

- Team Performance
- Player Analysis
- Match Trends
- Venue Analysis
- Toss Impact
- Batting & Bowling Metrics

---

# 📌 Project Objectives

The main objective of this project was to:

- Build a complete analytics workflow from raw dataset to interactive dashboard
- Perform proper data validation and cleaning
- Create analytics-ready tables using Python
- Design a professional multi-page Power BI dashboard
- Generate meaningful cricket insights through data storytelling

---

# 🛠️ Tools & Technologies Used

| Tool | Purpose |
|------|---------|
| Python | Data Cleaning & Preprocessing |
| Pandas | Data Manipulation |
| NumPy | Statistical Calculations |
| Power BI | Dashboard Creation |
| DAX | KPI & Measures |
| Power Query | Data Transformation |
| GitHub | Project Hosting & Documentation |

---

# 📂 Dataset Information

- **Dataset Type:** IPL Ball-by-Ball Dataset
- **Seasons Covered:** 2022–2025
- **Source:** Kaggle IPL Dataset (https://drive.google.com/drive/folders/1VWj4AYcZI6ReR-avey9v297lVbxs3yL2?usp=sharing)
- **Total Records:** ~70,000+ Ball-by-Ball Entries

### Dataset Includes:
- Match Details
- Batting Statistics
- Bowling Statistics
- Toss Information
- Venue Details
- Wicket Events
- Innings Data
- Match Results

---

# 🔄 Project Workflow

The project was completed in multiple stages:

```text
Raw Dataset
     ↓
Data Validation
     ↓
Data Cleaning
     ↓
Feature Engineering
     ↓
Analytics Table Creation
     ↓
Power BI Data Modeling
     ↓
Dashboard Development
     ↓
Insights
```


# 🧹 1. Data Cleaning & Transformation

The raw dataset was cleaned and transformed using Python.

## Cleaning Tasks Performed

### ✔️ Team Standardization
Example:
- Delhi Daredevils → Delhi Capitals
- Kings XI Punjab → Punjab Kings

### ✔️ Venue Cleaning
Fixed inconsistent venue names across seasons.

### ✔️ Null Handling
Handled:
- Review-related columns
- Empty columns
- Null-heavy features

### ✔️ Data Type Conversion
- Converted date columns
- Corrected numeric types
- Boolean conversion for analytics

---

# 🏗️ 2. Analytics-Ready Tables Created

The raw dataset was transformed into multiple structured tables for Power BI analysis.

---

## 📌 BallByBall Table

Main granular dataset where:

> **1 row = 1 delivery**

### Features Added
- Match Phase Classification
- Dot Ball Indicator
- Boundary Indicator
- Legal Wicket Indicator
- Display Over Formatting

### Used For
- Match Trends
- Batting Insights
- Bowling Insights

---

## 📌 MatchSummary Table

Match-level aggregated dataset where:

> **1 row = 1 match**

### Includes
- Teams
- Venue
- Toss Details
- Match Winner
- Innings Scores
- Match Result

### Used For
- KPI Cards
- Venue Analysis
- Toss Analysis
- Match Trends

---

## 📌 BatterStats Table

Player-level batting analytics table.

### Metrics Calculated
- Runs Scored
- Balls Faced
- Strike Rate
- Fours & Sixes
- Boundary %
- 50s & 100s

### Used For
- Orange Cap Analysis
- Batter Comparison
- Aggressive Batting Analysis

---

## 📌 BowlerStats Table

Player-level bowling analytics table.

### Metrics Calculated
- Wickets
- Economy Rate
- Dot Ball %
- Bowling Average
- 3W & 5W Hauls

### Used For
- Purple Cap Analysis
- Bowling Efficiency
- Pressure Bowling Analysis

---

## 📌 TeamPerformance Table

Team-level aggregated analytics table.

### Metrics Included
- Matches Played
- Matches Won
- Win Percentage
- Team Runs
- Team Wickets
- Boundary Counts

### Used For
- Team Comparison
- Team Success Analysis
- Performance Metrics

---

# 🔗 4. Power BI Data Modeling

The project follows a structured Power BI data model using relationships between analytical tables.

## Relationships Used

| From | To | Relationship |
|------|----|--------------|
| MatchSummary | BallByBall | One-to-Many |
| MatchSummary | BatterStats | One-to-Many |
| MatchSummary | BowlerStats | One-to-Many |
| Teams | TeamPerformance | One-to-Many |

---

# 📊 5. Dashboard Pages

The Power BI dashboard contains multiple analytical pages.

---

# 🏏 Page 1 — IPL Overview Dashboard

Provides a high-level overview of IPL analytics.

## Features
- Total Matches KPI
- Total Runs KPI
- Total Wickets KPI
- Total Sixes KPI
- Highest Team Score KPI
- Runs by Season Trend
- Top Batters
- Top Bowlers
- Toss Decision Analysis
- Venue-wise Average Score


---

# 🏆 Page 2 — Team Performance Analysis

Focused on team-level insights and comparison.

## Features
- Team-wise Win Percentage
- Matches Won Analysis
- Boundary Analysis
- Team Bowling Analysis
- Toss Impact
- Team Comparison Table
- Interactive Team Slicer

---

# 👤 Page 3 — Player Performance Analysis

Focused on batting and bowling performance.

## Features
- Orange Cap Leaders
- Purple Cap Leaders
- Boundary Percentage
- Dot Ball Percentage

---

# 📈 6. Key Insights 

Some major insights observed from the dashboard:


- Batting strike rates increased significantly in recent seasons
- Certain venues consistently produce higher first innings scores
- Teams winning toss often prefer chasing
- High dot-ball percentage bowlers usually maintain lower economy rates
- Boundary percentage helps identify aggressive finishers

---

# ⚡ 7. Key Power BI Features Used

## DAX Measures
Created custom measures for:
- Total Matches
- Total Runs
- Total Wickets
- Win Percentage
- Average Venue Score

---

## Interactive Features
- Dynamic Slicers
- Cross Filtering
- Tooltips
- Conditional Formatting
- Interactive Visuals

---

# 📁 Folder Structure

```text
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
│
├── notebooks/
│   └── data_cleaning.ipynb
│
├── README.md
```

---

# 📚 Learning Outcomes

This project helped strengthen my understanding of:

- Data Cleaning & Preprocessing
- Data Modeling in Power BI
- DAX Calculations
- Dashboard Design
- Data Storytelling
- Sports Analytics
- Interactive Visualization

---

# 📸 Dashboard Screenshots

## IPL Overview Dashboard

```md
![IPL Overview](images/dashboard_overview.png)
```

## Team Performance Dashboard

```md
![Team Analysis](images/team_analysis.png)
```

## Player Analysis Dashboard

```md
![Player Analysis](images/player_analysis.png)
```

---

# 📌 Project Files

## Power BI Dashboard
- `IPL_Dashboard.pbix`

## Dashboard PDF
- `IPL_Dashboard.pdf`

## Dataset
- IPL Ball-by-Ball Dataset (2022–2025)

---

# 🤝 Connect With Me

## LinkedIn
www.linkedin.com/in/divyanshuverma-career

## GitHub
https://github.com/divyanshuverma-career

---

# ⭐ Feedback

Feedback and suggestions are always welcome.

If you found this project useful or interesting, feel free to connect or share your thoughts.

⭐ If you liked this project, consider giving it a star on GitHub!
