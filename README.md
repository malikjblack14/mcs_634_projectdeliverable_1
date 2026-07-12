# Lab 1: Data Visualization, Data Preprocessing, and Statistical Analysis

## Purpose of Lab Work
The purpose of this lab is to perform initial data exploration, cleaning, preprocessing, and visualization on an Electric Vehicle (EV) Population dataset. This work establishes a baseline understanding of EV distributions, manufacturer dominance, and vehicle ranges to prepare the dataset for deeper data mining tasks.

## Key Insights from Visualizations
*   **Top 10 Electric Vehicle Makes (Bar Chart):** The visualization clearly demonstrates that Tesla heavily dominates the dataset with over 120,000 vehicles. Other manufacturers like Chevrolet, Nissan, and Ford follow but hold significantly smaller portions of the market share.
*   **Distribution of Electric Range (Histogram):** The data reveals a massive cluster of vehicles with a shorter range (0–50 miles), which represents plug-in hybrid models or early-generation EVs. A second, smaller distribution peak occurs around 200–250 miles, capturing modern, long-range battery electric vehicles.

## Key Insights from Statistical Analysis
*   **Descriptive Statistics:** The sampled dataset contains 24,401 vehicles with an average model year of ~2023. The average electric range is approximately 7.89 miles, with a high variance ($250.75$), reflecting the massive proportion of newer models that register a $0.0$ baseline range calculation or plug-in hybrids compared to high-range exceptions.
*   **Correlation Matrix:** There is a moderate negative correlation ($-0.466$) between `Model Year` and `Electric Range`. This indicates that as the model year increases (newer vehicles), the reported battery range value in this specific attribute decreases, likely due to a shift in how newer model data forms or a prevalence of newer hybrid models with smaller baseline standard electric-only ranges.

## Challenges Faced & Decisions Made
*   **Environment Configuration:** Encountered initial `ModuleNotFoundError` issues for `ipykernel`, `pandas`, `matplotlib`, and `seaborn`. This was resolved by dynamically installing the required packages directly within the Jupyter environment using `pip`.
*   **System Storage Limitations:** Ran into a critical `OSError: [Errno 28] No space left on device` during package installations due to a full hard drive. To resolve this, large cached installation files were cleared and purged from the system Trash to free up the necessary environment deployment space.
*   **File Path Calibration:** Dealt with a `FileNotFoundError` when loading the dataset. The file path was updated from a local root assumption to accurately reference the `Downloads/` directory where the source data was located.s