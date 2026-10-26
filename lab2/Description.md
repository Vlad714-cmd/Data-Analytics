# Barcelona FC Player Stats Analysis (Pandas & Data Analytics)

This repository contains a Data Analytics practical assignment focused on exploring, manipulating, and analyzing a football performance dataset (`messi barca.csv`) using **Python** and **Pandas** in **Google Colab**.

## 📌 Project Overview
The objective of this assignment is to demonstrate fundamental data analysis workflows, including data loading, inspection, filtering, custom grouping functions, and exporting processed outputs.

The dataset consists of **44 entries and 17 feature columns** covering seasonal match statistics, goals, assists, disciplinary metrics, and advanced normalized rates (e.g., per 90-minute stats).

---

## 🛠️ Key Tasks & Implementation

1. **Environment Setup & Data Loading:**
   * Mounted Google Drive to Google Colab.
   * Loaded the CSV dataset into a Pandas DataFrame using `utf-8` encoding (with error ignoring).

2. **Exploratory Data Analysis (EDA):**
   * Inspecting structure, column data types (`object`, `int64`, `float64`), and non-null values via `df.info()`.
   * Summary statistics calculation (mean, std, min, max, quartiles) using `df.describe()`.
   * Inspecting the first few rows (`df.head(3)`) and the last records (`df.tail(3)`) to verify data boundaries (e.g., spanning from the 2004-2005 to the 2019-2020 seasons).

3. **Data Selection & Indexing:**
   * Row-level inspection using label-based (`.loc[]`) and position-based (`.iloc[]`) indexing.
   * Target cell extraction across individual features.

4. **Filtering & Sorting:**
   * Boolean masking to filter rows matching performance conditions (e.g., goals scored thresholds).
   * Sorting DataFrame records in descending order using `.sort_values()`.

5. **Aggregation & Custom Functions:**
   * Created a reusable custom function (`group_and_sort_by_column`) utilizing `.value_counts()` and `.reset_index()` to aggregate and sort categorical variables such as `Competition`.
   * Successfully summarized match counts per tournament (e.g., Champions League, La Liga, Copa del Rey, Supercopa, and Super Cup).

6. **File Export:**
   * Exporting processed and filtered DataFrames to clean `.csv` files stored directly on Google Drive (`to_csv(index=False)`).

---

## 📂 Dataset Structure

* **Categorical / Text Columns (2):** `Season`, `Competition`
* **Integer Numeric Columns (10):** `Age`, `Matches Played`, `Starts`, `Minutes played`, `Goals scored`, `Assists`, `PK`, `PKatt`, `CrdY`, `CrdR`
* **Floating-Point Columns (5):** `Goal/90`, `Ast/90`, `G+A/90`, `G-PK/90`, `G+A-PK/90`

---
