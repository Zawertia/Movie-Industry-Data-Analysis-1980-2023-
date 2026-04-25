# Movie Industry Trends Analysis (1980-2023) 🎬📊

## 📌 Project Overview
This project focuses on extracting, cleaning, and analyzing a comprehensive dataset of Wikipedia movie data spanning over four decades. The goal is to identify shifting trends in cinematography, track the popularity of genres, and analyze the productivity of top actors throughout their careers.

## 🚀 Key Objectives
* **Data Integration:** Dynamically fetch and merge multiple JSON datasets from GitHub using `NumPy` and `Pandas`.
* **Data Transformation:** Handle nested JSON structures (lists of genres and cast) into a flat format suitable for analysis.
* **Trend Analysis:** Visualize how the popularity of "Big Three" genres changed year-over-year.
* **Actor Productivity:** Identify top performers and analyze their genre preferences (Top Genres vs. Others).

## 🛠 Tech Stack
* **Language:** Python 3.x
* **Data Processing:** `Pandas`, `NumPy`
* **Data Parsing:** `json`, `ast` (Literal Evaluation for stringified lists)
* **Visualization:** `Matplotlib` (Line charts, Bar charts, Stacked charts, Pie charts)

## 📈 Analysis Highlights
1.  **Dynamic Data Loading:** Automated the retrieval of datasets from 1980 to 2023 by generating URL sequences with `np.arange`.
2.  **Advanced Data Cleaning:** * Removed redundant metadata (thumbnails, hrefs).
    * Filtered out incomplete records while preserving rows with partial data (e.g., movies with cast but no genre) to maximize data utility.
3.  **Exploratory Data Analysis (EDA):**
    * **Genre Explosion:** Flattened nested lists to rank the Top 10 genres.
    * **Time-Series Analysis:** Visualized the rise and fall of genres like Drama, Comedy, and Action over 40 years.
    * **Actor Insights:** Tracked the career trajectories of legendary actors (e.g., Samuel L. Jackson, Robert De Niro) using `pivot_table` logic.
4.  **Bonus Feature - Genre Proportions:** Calculated the ratio of "Top-3 Genres" vs. "Other Genres" for the most prolific actors, visualized through a Stacked Bar Chart.

## 📂 Project Structure
- `пирогова_дз_12.py` - Core script including data fetching, cleaning, and visualization.
- `combined_dataset_movies_1980-2023.csv` - The processed final dataset used for analysis.

## 💡 Results & Conclusions
The analysis revealed significant shifts in the film industry:
* **Genre Dominance:** While Drama and Comedy remain staples, Action and Sci-Fi showed distinct peaks during specific decades.
* **Actor Versatility:** Top actors often maintain a consistent balance between mainstream genres and niche projects, though some (like Jackie Chan) show a clear dominance in specific categories.
