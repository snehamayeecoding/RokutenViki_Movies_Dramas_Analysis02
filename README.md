# Rakuten Viki Movies & Dramas — Data Cleaning & Exploratory Data Analysis (Python)

> 🔗 **Related Analysis:** Check out Part 1 of this project using **T-SQL (SQL Server)** [here](https://github.com/snehamayeecoding/RokutenViki_Movies_Dramas_Analysis).

## 📌 Project Overview
An end-to-end data cleaning, feature engineering, and exploratory data analysis (EDA) project on the **Rakuten Viki Movies & Dramas** catalog (`titles`). Building on my initial SQL analysis, this Python repository cleans messy data by statistically analysing the numeric columns, exploding the `genres` and `production countries` columns , explores useful insights by building beautiful visualizations using `matplotlib` and `seaborn`.

## 📁 Repository Structure
* `notebooks/01_data_cleaning_and_eda.ipynb` : Complete Python workflow for data cleaning, list parsing, statistical exploration, and visualization.
* `data/` : Raw and processed datasets exported for downstream BI reporting (`cleaned_titles`, `genres_exploded`, `countries_exploded`, `genres_and_countries`).
* `README.md` : Project documentation, methodology, and key analytical findings.

## 🛠️ Tools & Libraries
* **Language:** Python 3
* **Data Manipulation:** Pandas, NumPy, Regular Expressions/ String Manipulation
* **Data Visualization:** Matplotlib, Seaborn
* **Environment:** VS Code / Jupyter Notebook

## 🔄 Data Cleaning & Processing Pipeline
1. **Data Auditing & Missing Value Treatment:** Handled null values across release years, age certifications, runtime, and cast/crew credits.
2. **Parsing Nested Structures:** Converted stringified list columns (`genres` and `production_countries`) into clean Python lists and exploded them into normalized tables for multi-dimensional analysis.
3. **Export for BI & Modeling:** Saved clean, analysis-ready CSV datasets (`cleaned_titles`, `genres_exploded`, etc.) to power an interactive Power BI dashboard and an ML recommendation system.

## 📊 Key Analytical Insights 
* **1. Content type and Genres Dominance by Volume:** `Dramas` dominate `Movies` in the platform and `Drama`, `Romance` and `Comedy` are the most dominating genres in the catalog.
* **2. Production Country Dominance:** Korea(**KR**), China(**CN**) and Japan(**JP**) are the major production countries.
* **Genre Dominance by IMDb Score and Votes:** Though Drama, Romance and Comedy top the genre list by volume , on the basis of IMDb score and votes `History` and `Sci-fi` tops the list followed by `Reality`, `Music` and `Romance`(well Romance keeps its position in top 5 with an average IMDb score of 7.18)

## 🚀 Next Steps
* **Power BI Dashboard:** Building an interactive executive report using the exported `cleaned_titles` and exploded tables.
* **ML Recommendation System:** Developing a title-based recommendation engine on the cleaned Rakuten Viki catalog.
*