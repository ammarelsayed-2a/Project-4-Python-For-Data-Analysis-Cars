# Project-4-Python-For-Data-Analysis-Cars
End-to-end EDA project on a real-world Cars dataset | Data cleaning, filtering &amp; transformation using Python, Pandas, Matplotlib &amp; Seaborn including fillna, isin, apply &amp; value_counts for exploratory data analysis

# 🚘 Data Analysis Project — Cars Dataset

A hands-on Data Analysis project on a real-world Cars dataset (432 vehicles), completed as part of the **Python for Data Analysis** course.

## 📌 Objective
Practice core Pandas operations — data cleaning, filtering, and transformation — while building a complete EDA with visualizations and actionable insights.

## 📂 Dataset
- **Source:** CarsData.csv
- **Records:** 432 vehicles
- **Features:** Make, Model, Type, Origin, DriveTrain, MSRP, Invoice, EngineSize, Cylinders, Horsepower, MPG_City, MPG_Highway, Weight, Wheelbase, Length

## 🛠️ Tools & Libraries
| Library | Purpose |
|---|---|
| Pandas | Data cleaning, filtering, transformation |
| Matplotlib | Base plotting |
| Seaborn | Statistical visualizations |

## 🔧 Pandas Commands Covered
| Command | Purpose |
|---|---|
| `pd.read_csv()` | Load CSV file into a DataFrame |
| `head()` | Show first N rows (default 5) |
| `shape` | Show total rows and columns |
| `isnull().sum()` | Detect missing values per column |
| `fillna()` | Fill null values with a specified value or mean |
| `value_counts()` | Count occurrences of each unique value |
| `isin()` | Filter rows matching values in a list |
| `apply()` | Apply a custom function along a column or row |

## ❓ Analytical Questions

### Q1 — Data Cleaning: Fill Null Values with Column Mean
Find all null values in the dataset. Fill numerical nulls with the column mean, and categorical nulls with the column mode.

### Q2 — Value Counts: Different Types of Car Makes
Check all unique Makes in the dataset and the count of each occurrence.

### Q3 — Filtering: Show records where Origin is Asia or Europe
Use `isin()` to filter only Asian and European cars.

### Q4 — Remove rows where Weight > 4000
Drop all records where the car's weight exceeds 4000 using the `~` (NOT) operator.

### Q5 — Increase all MPG_City values by 3
Use `apply()` with a lambda function to add 3 to every value in the MPG_City column.

## 📊 Analysis Structure
1. Imports & Setup
2. Load Dataset
3. First Look (head / tail)
4. Data Structure & Info
5. Descriptive Statistics
6. Categorical Exploration
7. Analytical Questions (Q1 → Q5)
8. Visualizations
   - Univariate (Numerical + Categorical)
   - Bivariate (Num vs Num · Num vs Cat · Cat vs Cat)
   - Multivariate
   - Correlation Heatmap · Pairplot
9. Key Insights

## 💡 Key Insights
- Strong positive correlation between Weight and Horsepower
- Higher horsepower leads to lower city fuel efficiency (MPG_City)
- Asian cars are the most fuel-efficient by Origin
- Sports cars lead in horsepower; Trucks lead in weight
- USA dominates SUV and Truck segments; Asia leads in Sedans
- Over 20% of records had Weight > 4000 — mostly Trucks and large SUVs

## 🚀 How to Run
```bash
git clone https://github.com/ammarelsayed-2a/Project-4-Python-For-Data-Analysis-Cars.git
cd Project-4-Python-For-Data-Analysis-Cars
jupyter notebook "Project 4 Cars.ipynb"
```

## 👤 Author
**Ammar Elsayed** — Python for Data Analysis | 2026  
[LinkedIn](https://www.linkedin.com/in/ammar-elsayed-ibrahim)
