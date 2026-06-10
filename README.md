# Project-4-Python-For-Data-Analysis-Cars
End-to-end EDA project on a real-world Cars dataset | Data cleaning, filtering &amp; transformation using Python, Pandas, Matplotlib &amp; Seaborn including fillna, isin, apply &amp; value_counts for exploratory data analysis

# 🚗 Exploratory Data Analysis — Cars Dataset

A structured EDA project on a real-world Cars dataset, completed as part of the Python for Data Analysis course.

## 📌 Objective
A structured EDA project on a real-world Cars dataset, completed as part of the Python for Data Analysis course.

Practice core Pandas operations — data cleaning, filtering, and transformation — while building a complete exploratory data analysis (EDA) with visualizations and actionable insights.

Explore and understand the dataset through statistical summaries and visual analysis, covering data structure, distributions, relationships, and key patterns.

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

After analyzing **432 car records** across 15 features:

1. **Heavier cars have significantly more horsepower**  
   There is a strong positive correlation between Weight and Horsepower — confirmed by both the scatter plot and the correlation heatmap.

2. **More horsepower = lower fuel efficiency**  
   MPG_City has a clear negative correlation with Horsepower and EngineSize — high-performance cars consume more fuel in city driving.

3. **Asian cars are the most fuel-efficient**  
   The barplot of MPG_City by Origin shows Asian cars lead in city fuel efficiency, followed by European cars, with USA cars trailing behind.

4. **Sports cars dominate in horsepower, Trucks in weight**  
   The boxplot of Horsepower by Type reveals Sports cars have the highest median horsepower, while Trucks are the heaviest category.

5. **USA dominates SUV and Truck segments**  
   The categorical countplot shows that most SUVs and Trucks in the dataset originate from the USA, while Asia leads in Sedans.

6. **Over 20% of records had Weight > 4000**  
   Before filtering, a substantial portion of records exceeded the 4000 weight threshold — mostly Trucks and large SUVs from USA manufacturers.


## 🚀 How to Run
```bash
git clone https://github.com/ammarelsayed-2a/Project-4-Python-For-Data-Analysis-Cars.git
cd Project-4-Python-For-Data-Analysis-Cars
jupyter notebook "Project 4 Cars.ipynb"
```

## 👤 Author
**Ammar Elsayed** — Python for Data Analysis | 2026  
[LinkedIn](https://www.linkedin.com/in/ammar-elsayed-ibrahim)
