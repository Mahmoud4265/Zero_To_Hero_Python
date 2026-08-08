# 🐼 Pandas Mastery: 60 Puzzles Challenge

<div align="center">

![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white)
![Jupyter](https://img.shields.io/badge/Jupyter-F37626?style=for-the-badge&logo=jupyter&logoColor=white)
![Status](https://img.shields.io/badge/Status-Completed-success?style=for-the-badge)

<p align="center">
  <b>A comprehensive hands-on practice solving the famous 60 Pandas Puzzles to master data manipulation & analysis in Python.</b>
</p>

</div>

---

## 📌 Overview

This repository contains step-by-step solutions for the well-known **Pandas Puzzles** (60 core questions). These exercises cover essential data manipulation techniques using `pandas`—from foundational DataFrame creations and filtering to complex aggregations, time series, and performance optimizations.

---

## 🚀 Key Topics Covered

- [x] **DataFrame Basics:** Creation, indexing, selecting columns, and inspecting metadata (`info()`, `describe()`).
- [x] **Data Cleaning:** Handling missing values (`NaN`), string formatting, and type conversions.
- [x] **Filtering & Selection:** Querying data using `.loc`, `.iloc`, boolean indexing, and multiple conditions.
- [x] **Aggregations & Grouping:** Using `.groupby()`, `.agg()`, pivot tables, and custom grouping logic.
- [x] **Data Transformation:** Applying functions via `.apply()`, `.map()`, and handling string operations.
- [x] **Time Series & Datetime:** Resampling, date ranges, shifted windows, and rolling calculations.

---

## 📂 Project Structure

```text
100-pandas-puzzles/
│
├── 60-pandas-questions.ipynb   # Complete Jupyter Notebook with solved puzzles & commentary
└── README.md                   # Project documentation & reference guide
```
💻 Quick Start
To run the solutions locally on your machine:

1.Clone the repository:

```Bash
git clone [https://github.com/Mahmoud4265/Zero_To_Hero_Python.git](https://github.com/Mahmoud4265/Zero_To_Hero_Python.git)
```
2.Navigate to the directory:

```Bash
cd Zero_To_Hero_Python/Pandas_Mastery/100-pandas-puzzles
```
3.Install dependencies:

```Bash
pip install pandas numpy jupyter
```
Launch Jupyter Notebook:

```Bash
jupyter notebook
```
🏆 Key Takeaways & Learned Techniques

Core Insight: Mastering vectorization in Pandas avoids slow Python loops (for loops) and leverages underlying C-level performance through NumPy.

Some crucial concepts practiced:

 - Avoiding chained indexing by using .loc[row, col] explicitly.

 - Efficient usage of .groupby().transform() for broadcasted group statistics.

 - Cleaning untidy data using .melt() and .pivot_table().

Crafted with 💡 as part of the Zero To Hero Python Data Science Roadmap.
