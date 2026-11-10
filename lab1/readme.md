# Practical Work №3: Data Cleaning, Transformation, and Feature Engineering

This repository contains materials and code for completing Practical Work №3 for the **Data Analytics** course. The work is dedicated to raw data preprocessing, handling missing values, outliers, and preparing the dataset for machine learning.

---

## 📋 Table of Contents
1. [General Information](#-general-information)
2. [Workflow Structure and Execution Steps](#-workflow-structure-and-execution-steps)
3. [Tech Stack](#-tech-stack)
4. [Running Instructions](#-running-instructions)
5. [Results and Saved Files](#-results-and-saved-files)

---

## 🎯 General Information
* **Contributors:** Vlad and teammates (Artur, Andrii, Vasylka, Kharechko)
* **Domain Area:** Sports statistics analysis (based on Lionel Messi's match dataset for FC Barcelona).
* **Objective:** Gain practical skills in identifying and resolving missing values, handling duplicates, filtering outliers using the Interquartile Range (IQR) method, encoding categorical variables (One-Hot Encoding), normalizing/standardizing numerical features, and automating processes via functions.

---

## ⚙️ Workflow Structure and Execution Steps
The script and notebook implement the following steps:
1. **Loading and Initial Review:** Reading `messi barca.csv` with encoding handling (`utf-8` / `latin1`), checking for duplicates and missing values.
2. **Data Cleaning:** Removing full duplicates, filling missing values with the median (for numeric columns) and the mode (for categorical columns).
3. **Text Operations:** Standardizing tournament names (converting to lowercase, stripping extra spaces).
4. **Feature Engineering:** 
   - Extracting the season's start year.
   - Calculating total goal contributions per match (`G+A_per_match`).
   - Creating a binary flag `is_top_scoring_season` using `np.where()`.
5. **Categorical Encoding:** Applying One-Hot Encoding (`pd.get_dummies`) to the tournament column.
6. **Normalization and Standardization:** Min-Max scaling (`[0, 1]`) and Z-score standardization for the goals scored metric (`Goals scored`).
7. **Universal Function:** Writing and testing the `clean_dataset(df)` function, which automates the entire cleaning pipeline for new datasets.

---

## 🛠 Tech Stack
* **Programming Language:** Python 3.13
* **Data Analysis Libraries:** 
  * `Pandas` — for table and DataFrame manipulation
  * `NumPy` — for vector computations and array operations
* **Execution Environment:** Google Colab / Jupyter Notebook
* **Version Control System:** Git (with release tagging)