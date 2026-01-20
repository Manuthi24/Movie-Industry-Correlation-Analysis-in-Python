# 🎬 Movie Industry Exploratory Data Analysis (EDA)

## 📌 Project Overview
This project is a **technical Exploratory Data Analysis (EDA)** focused on identifying the variables that most significantly impact the **gross revenue of films**.

Using a real-world movie industry dataset, the analysis investigates factors such as **budget**, **production company**, and **user votes** to determine how strongly they correlate with a movie’s **financial success**. The project demonstrates practical data cleaning, visualisation, and correlation analysis using Python.

---

## 📂 Dataset
The dataset used in this project is the **Movie Industry Dataset**, sourced directly from **Kaggle**. It contains **15 columns** describing various attributes of films.

### Key Features:
- **Budget** – Cost to produce the film  
- **Gross** – Total revenue earned  
- **Company** – Production studio  
- **Votes** – Number of user votes received  
- **Released** – Release date and country  
- **Star, Writer, Director, Genre**

---

## 🛠 Tools & Libraries
This project was completed in a **Jupyter Notebook** environment using **Anaconda**.

- **Pandas** – Data manipulation and DataFrames  
- **NumPy** – Numerical operations  
- **Matplotlib** – Basic plotting and styling  
- **Seaborn** – Advanced statistical visualisation  

---

## 🔄 Project Workflow

### 1️⃣ Data Cleaning & Preparation
- **Missing Data Analysis:**  
  Iterated through all columns to identify and calculate the percentage of null values.
- **Data Type Correction:**  
  Converted `budget` and `gross` columns from floats to integers to remove unnecessary decimals.
- **Year Synchronisation:**  
  Created a new column `yearcorrect` by extracting the year from the `released` field, as the original `year` column was often inconsistent.
- **Sorting:**  
  Sorted the dataset by `gross` revenue in descending order to identify top-performing films.
- **Duplicate Handling:**  
  Checked for and removed duplicate records to maintain data integrity.

---

### 2️⃣ Exploratory Data Analysis & Visualisation
- **Scatter Plot:**  
  Created a scatter plot (Budget vs Gross) using Matplotlib to observe overall trends.
- **Regression Plot:**  
  Used Seaborn to generate a regression plot, visually confirming a **positive relationship** between budget and gross revenue.

---

### 3️⃣ Correlation Analysis
- **Correlation Matrix:**  
  Generated correlation matrices using:
  - Pearson (default)
  - Kendall
  - Spearman
- **Heatmap Visualisation:**  
  Used a Seaborn heatmap to clearly identify strong and weak correlations.
- **Categorical Numerisation:**  
  Converted non-numeric fields (e.g., company, genre) into numeric category codes to include them in the full correlation analysis.
- **Unstacking Correlations:**  
  Unstacked and sorted correlation pairs to quickly identify the highest correlation coefficients.

---

## 📊 Key Insights
- **Budget vs Gross Revenue:**  
  A strong positive correlation (~**0.71**) exists, indicating that higher-budget movies generally earn more revenue.
- **Votes vs Gross Revenue:**  
  User engagement (votes) shows a significant correlation with financial success.
- **Company Influence:**  
  Contrary to the initial hypothesis, the production company had **low correlation** with gross revenue.

---

## 🎯 Project Outcome
- Identified the **key drivers of movie revenue** using statistical analysis
- Demonstrated **real-world EDA techniques** used in data analytics and data science
- Showcased effective **data cleaning, visualisation, and correlation analysis** in Python

---



<p align="center">
  <em>Exploratory Data Analysis turns raw data into actionable insights.</em>
</p>
