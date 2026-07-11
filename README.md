# MCS 634: Project Deliverable 1 - Data Collection, Cleaning, and Exploration

## Dataset Summary
This project analyzes NBA player performance statistics using data collected from the 2025-2026 basketball season. The raw dataset (`nba_player_stats.csv`) tracks key metrics across multiple athletes, including points scored, assists, rebounds, minutes played, and shooting percentages. The objective of this deliverable is to establish a solid foundation for predictive data mining and big data analytics by compiling, formatting, and analyzing this performance data.

## Data Cleaning & Exploration Steps
To ensure data integrity for subsequent data mining phases, the following structured preprocessing pipeline was executed inside `deliverable1.ipynb`:
* **Handling Missing Values:** Inspected the dataset for null values, duplicates, and structurally inconsistent records, applying appropriate imputation strategies where needed.
* **Feature Formatting:** Standardized numerical columns and categorical variables to maintain uniformity across player rows.
* **Exporting Cleaned Data:** Saved the processed results into a separate file (`nba_player_stats_cleaned.csv`) to keep raw and clean assets separate.
* **Data Exploration & Visualizations:** Conducted exploratory data analysis (EDA) using Matplotlib/Seaborn to generate clear, well-labeled charts (such as scoring distributions) to isolate key performance trends.

## Challenges Encountered & Resolutions
* **Challenge:** Managing inconsistent data formatting and structural null values within specific advanced metrics rows, which threatened to skew the overall exploratory visualizations.
* **Resolution:** Implemented localized filtering and data-type normalization scripts in Python to drop or safely impute corrupted fields, isolating the anomalies without compromising the broader dataset.
