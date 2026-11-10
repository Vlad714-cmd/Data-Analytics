# Practical Work No. 4: Data Aggregation and Grouping in Pandas

## Overview
This repository contains the completion of **Practical Work No. 4**, focusing on data manipulation, grouping, and aggregation techniques using Python's `pandas` library. The practical tasks demonstrate how to summarize, pivot, and merge datasets to calculate analytical indicators.

---

## Objectives
- Master the `groupby()` method and apply built-in aggregate functions (`sum`, `mean`, `count`, `min`, `max`).
- Build pivot tables using `pivot_table()` and cross-tabulations using `crosstab()`.
- Merge and combine datasets using `merge()`, `concat()`, and `join()`.
- Compute analytical summary metrics by groups and interpret results.
- Export aggregated outputs into CSV format.

---

## Dataset Description
The analysis was performed on a dataset containing detailed player performance statistics across multiple seasons and competitions. Key attributes include:
- `Season`: Competition season identifier.
- `Age`: Player age during the season.
- `Competition`: Name of the league or tournament.
- `Matches Played` / `Starts`: Number of appearances.
- `Minutes played`: Total playing time on the pitch.
- `Goals scored` / `Assists`: Offensive performance indicators.
- `PK` / `PKatt`: Penalty kick metrics.
- `CrdY` / `CrdR`: Disciplinary records (Yellow/Red cards).

---

## Tasks Completed

### Part 1: Core Tasks (Steps 1–10)
1. **Data Loading & Preparation:** Environment setup and loading dataset into Pandas DataFrame.
2. **Single-Column Grouping:** Aggregated total goals and average playing time by season.
3. **Multi-Column Grouping:** Analyzed match counts across seasons and competitions (`reset_index()`).
4. **Multiple Aggregation Functions:** Applied `agg(['sum', 'mean', 'min', 'max'])` to analyze goal distribution across tournaments.
5. **Pivot Tables:** Constructed pivot tables comparing performance by competition and player age.
6. **Cross-Tabulations:** Generated frequency distributions of matches per competition per season using `crosstab()`.
7. **Merging Data (`merge`):** Joined tournament categorization metadata using left joins.
8. **Concatenating Data (`concat`):** Merged split datasets vertically while preserving index integrity.
9. **Index-Based Join (`join`):** Demonstrated joining datasets based on index alignment.
10. **Analytical Metrics:** Computed relative contribution percentages of goals scored in each tournament relative to total goals.

### Part 2: Individual Assignments
- Executed customized grouping queries adapted to the dataset structure.
- Calculated overall record counts, minimum/maximum statistical bounds, multi-variable pivot tables, and derived metric calculations (e.g., total direct goal contributions $G + A$).

### Part 3: Additional Task
- Created a custom relational dataset containing team profiles and match performance metrics.
- Merged tables via `merge()`.
- Calculated three aggregate indicators (`sum`, `mean`, `count`).
- Created a summary pivot table and exported the final output to `football_summary.csv`.
