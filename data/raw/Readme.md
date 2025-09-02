# 🔗 Data Source

The analysis is based on the **2024 Divvy Trip Data**, made publicly available by Motivate International Inc.

- **Official Data Page:** [https://divvy-tripdata.s3.amazonaws.com/index.html](https://divvy-tripdata.s3.amazonaws.com/index.html)
- **License Agreement:** [Divvy Data License Agreement](https://ride.divvybikes.com/data-license-agreement)

## 📁 Dataset Details

To replicate the analysis, you must download the following files:

- **Time Period:** January 2024 - December 2024
- **Files Required (12):**
  - `202401-divvy-tripdata.zip`
  - `202402-divvy-tripdata.zip`
  - `202403-divvy-tripdata.zip`
  - `202404-divvy-tripdata.zip`
  - `202405-divvy-tripdata.zip`
  - `202406-divvy-tripdata.zip`
  - `202407-divvy-tripdata.zip`
  - `202408-divvy-tripdata.zip`
  - `202409-divvy-tripdata.zip`
  - `202410-divvy-tripdata.zip`
  - `202411-divvy-tripdata.zip`
  - `202412-divvy-tripdata.zip`

## 🚀 How to Use This Data

1.  **Download:** Click on each file name from the official data page (link above).
2.  **Extract:** Unzip each file to obtain the CSV files.
3.  **Place in Project Structure:** Move the extracted CSV files to the `/data/raw/` directory of this project.
4.  **Run the Code:** Execute the `01_data_cleaning.ipynb` Jupyter notebook to process the data and load it into the SQLite database. The SQL queries in this folder can then be run on that database.

## ℹ️ Note on File Size

The original CSV files are very large (over 5 GB combined) and are therefore not included in this GitHub repository. This is a standard practice to keep the repository efficient and manageable.

---

