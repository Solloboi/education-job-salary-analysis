# 📊 Dataset: Education Level, Job Category, and Annual Salary

This dataset contains records of individuals with varying levels of education and job categories, along with their reported **annual salaries in USD**. It is designed for use in data analysis and machine learning tasks that explore how education level and job type impact income.

---

## 🎯 Objective

The primary goal of this dataset is to:

- Analyze the relationship between **education level**, **job category**, and **annual salary**
- Identify groups of workers with the **highest** and **lowest** income levels
- Support studies on **wage inequality**, **career progression**, and **economic mobility**

---

## 🧩 Features

Each row in the dataset includes the following fields:

- `EducationLevel`: The highest level of education attained (e.g., *High School*, *Bachelor’s*, *Master’s*, *PhD*)
- `JobCategory`: The general job category or professional field (e.g., *Management*, *Technician*, *Administrative*)
- `AnnualSalary`: The reported yearly income in USD (stored as a float value, e.g., `50200.0`)

---

## 💡 Potential Use Cases

- 📈 **Regression analysis** to model salary based on education and job type
- 📊 **Data visualization** of salary distribution across education/job groups
- 🔍 **Clustering** or **classification** of workers based on income profiles
- 🌐 **Social research** on wage gaps and labor market trends

---

## 📂 Dataset Format

The dataset is stored as a CSV file: [`SalaryData.csv`](./SalaryData.csv)

Example rows:

| EducationLevel | JobCategory     | AnnualSalary |
|----------------|------------------|---------------|
| Bachelor’s     | Management        | 70450.0       |
| High School    | Technician        | 40100.0       |
| Master’s       | Administrative    | 55000.0       |

---

## 🛠 How to Use

### Python Example
```python
import pandas as pd

# Load the dataset
df = pd.read_csv("SalaryData.csv")

# Basic statistics
print(df.describe())

# Group by EducationLevel
print(df.groupby("EducationLevel")["AnnualSalary"].mean())
