# Cyclistic Bike-Share Analysis

## 🎯 1. Business Task

The goal of this analysis is to identify **how annual members and casual riders use Cyclistic bikes differently**. By analyzing behavioral patterns from the complete 2024 trip data, this project will provide actionable insights to guide the marketing team's strategy for converting casual riders into annual members, thereby driving future growth.

**Key Questions to Explore:**

* How do ride durations differ between members and casual riders?
* What are the patterns in ride volume by day of the week and time of day for each group?
* Which stations are most popular for casual riders, and how does this compare to members?
* Does bike type (classic, docked, electric) preference vary between the two groups?

## 👥 2. Stakeholders

* **Lily Moreno:** Director of Marketing (Primary stakeholder)
* **Cyclistic Marketing Analytics Team**
* **Cyclistic Executive Team** (Will approve the final strategy)

## 📊 3. Data Source

This analysis uses the most recent 12 months of Cyclistic trip data (Jan-Dec 2024).

* **Source:** [Divvy Trip Data](https://divvy-tripdata.s3.amazonaws.com/index.html)
* **License:** Data provided by Motivate International Inc. under this [license](https://ride.divvybikes.com/data-license-agreement).
* **Privacy:** All personally identifiable information has been removed. Analysis focuses solely on aggregate behavioral patterns.

## 🗂️ 4. Repository Structure

```
cyclistic-bikeshare-analysis/
│
├── data/
│   ├── raw/       # Original, unaltered source CSV files (12 files)
│   └── clean/     # Processed data in Parquet format & SQL database
│
├── notebooks/     # Jupyter notebooks for the analysis process
│   ├── 01_data_cleaning.ipynb
│   ├── 02_sql_analysis.ipynb
│   └── 03_visualization.ipynb
│
├── sql/           # Standalone SQL query files for analysis
│
├── outputs/
│   ├── tables/    # Exported summary tables (CSV)
│   └── figures/   # Exported visualizations (PNG)
│
├── data_cleaning_log.md # Summary of data cleaning steps & changes
└── README.md            # Project overview (this file)
```

## 🔧 5. Tools & Technologies

* **Data Processing & Cleaning:** Python (Pandas, NumPy)
* **Database & Analysis:** SQLite, SQL
* **Visualization:** Python (Matplotlib, Seaborn), Tableau Public
* **Version Control & Documentation:** Git, GitHub, Markdown

## 🔄 6. Process

The analysis will follow the six steps of the data analysis process: **Ask, Prepare, Process, Analyze, Share, and Act.**

1. **Ask:** Define the business task and key questions. *(Complete)*
2. **Prepare:** Identify and download data; set up the project structure. *(Complete)*
3. **Process:** Clean and transform the data for analysis. This includes:

   * Combining 12 monthly files into a single dataset.
   * Calculating new columns (ride\_length, day\_of\_week, month, etc.).
   * Filtering out invalid data (negative times, rides >24 hours).
   * Documenting all cleaning steps in a log.
   * Loading the clean data into an SQL database for analysis.
4. **Analyze:** Use SQL and Python to perform exploratory data analysis (EDA) and identify trends.
5. **Share:** Create visualizations and build a dashboard to communicate findings.
6. **Act:** Provide top three data-driven recommendations for the marketing strategy.

---
## 📊 7. Analysis & Key Findings

The analysis phase involved running targeted SQL queries on the cleaned database to answer the core business questions. The following key insights were uncovered:

**1. Ride Duration:**
- Casual riders take **70% longer** trips on average (20.9 minutes) compared to members (12.2 minutes), indicating a leisure-oriented usage pattern.

**2. Weekly Patterns:**
- **Members** show consistent, high usage throughout the **weekdays** (M-F), characteristic of commuting.
- **Casual** ridership spikes significantly on **weekends** (Sat-Sun), confirming use for leisure activities.

**3. Daily Patterns:**
- Member traffic shows distinct **rush hour peaks** at 7-8 AM and 4-6 PM.
- Casual ridership builds gradually, peaking in the **early afternoon** (2-4 PM).

**4. Geographic Trends:**
- The top 10 stations for casual riders are overwhelmingly concentrated around **Chicago's major tourist and recreational attractions** (e.g., Navy Pier, Millennium Park, Shedd Aquarium, Adler Planetarium).

**5. Bike Type Preference:**
- While both groups use classic and electric bikes, **casual riders were the primary users of electric scooters**, suggesting a willingness to try new mobility options.

*These findings were exported to CSV files for further visualization and are available in the `/outputs/tables/` directory.*
*This project is part of the Google Data Analytics Professional Certificate. Cyclistic is a fictional company, but the data has been made available by Motivate International Inc.*
