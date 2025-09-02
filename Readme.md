# Cyclistic Bike-Share Analysis: From Data to Strategy

## 🎯 1. Business Task

The primary goal of this analysis is to **identify and analyze the key behavioral differences** between Cyclistic's annual members and casual riders using the complete 2024 trip data. The insights derived will directly inform the marketing team's strategy to design targeted initiatives aimed at converting casual riders into profitable annual members.

**Final Task Statement:**
> "To analyze how annual members and casual riders use Cyclistic bikes differently by examining their 2024 riding patterns to identify key behavioral differences for a targeted marketing strategy."

---

## 👥 2. Key Stakeholders

- **Lily Moreno:** Director of Marketing (Primary stakeholder and project sponsor)
- **Cyclistic Marketing Analytics Team:** Responsible for analysis and reporting
- **Cyclistic Executive Team:** Will review and approve the final strategic recommendations

---

## 📁 3. Data Source and Description

**Data Source:** [Divvy Trip Data](https://divvy-tripdata.s3.amazonaws.com/index.html) provided by Motivate International Inc.

**License:** This data is made available under the [Divvy Data License Agreement](https://ride.divvybikes.com/data-license-agreement).

**Dataset Details:**
- **Time Period:** January 2024 - December 2024 (12 months)
- **Files Used:** 12 monthly ZIP files (`202401-divvy-tripdata.zip` to `202412-divvy-tripdata.zip`)
- **Privacy Note:** All personally identifiable information has been removed in compliance with data privacy regulations.

---

## 🗃️ 4. Repository Structure

The project is organized as follows:

```
cyclistic-bikeshare-analysis/
│
├── 📊 data/
│   ├── 📂 raw/               # Original, immutable source data (12 CSV files)
│   └── 📂 clean/             # Processed data (Parquet, SQLite DB)
│
├── 📓 notebooks/             # Jupyter notebooks for analysis
│   ├── 01_data_cleaning.ipynb
│   ├── 02_sql_analysis.ipynb
│   └── 03_visualization.ipynb
│
├── 🗃️ sql/                   # SQL query files for analysis
│   ├── rides_by_month.sql
│   ├── avg_ride_length.sql
│   └── ...
│
├── 📈 outputs/
│   ├── 📂 tables/            # Exported summary tables (CSV)
│   └── 📂 figures/           # Exported visualizations (PNG)
│
└── README.md                 # Project overview and documentation
```

---

## 🔧 5. Tools & Technologies

- **Data Processing & Analysis:** Python (Pandas, NumPy), SQL
- **Database Storage:** SQLite
- **Visualization:** Python (Matplotlib, Seaborn), Tableau Public
- **Version Control:** Git, GitHub

---

## 🚀 Next Steps

With the data downloaded and the repository structure in place, the next phase is:
1.  **Data Processing:** Clean the raw CSVs, calculate new fields (`ride_length`, `day_of_week`, etc.), and load into an SQLite database.
2.  **Analysis:** Perform exploratory data analysis (EDA) using SQL queries to uncover trends.
3.  **Visualization:** Create compelling visualizations to communicate key insights.
4.  **Recommendations:** Formulate three data-driven marketing strategies for presentation to the executive team.

---

### What You've Accomplished So Far (You are right on track!):

✅ **Defined the "Ask" Phase:** You have a clear business task and know your stakeholders.  
✅ **Prepared the Data:** You've identified the source and downloaded the 12 files for 2024.  
✅ **Set Up Project Structure:** You've created the folder paths.  
✅ **Connected to GitHub:** Your local folder is linked to your remote repo.

### What's Left for Day 1:

1.  **Move the ZIP files:** Place the 12 downloaded `2024XX-divvy-tripdata.zip` files into your `/data/raw/` folder.
2.  **Unzip them:** Extract all 12 CSV files into that same `/data/raw/` folder. You should have `202401-divvy-tripdata.csv`, `202402-divvy-tripdata.csv`, etc., in there.
3.  **Create the README.md:** Copy the text above into a new file named `README.md` in your main project folder.
4.  **Push to GitHub:** Add, commit, and push this new `README.md` file and your folder structure (with the raw data) to GitHub.

You have done the most important part—the planning. Now you are perfectly set up to start the data processing on Day 2.
## 📊 Key Analysis Questions
1. How does average ride duration differ between members and casual riders?
2. Are there peak usage times/days for each group?
3. Which stations are most popular for casual riders?
4. How does bike type (classic vs. electric) preference vary?