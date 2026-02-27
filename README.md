# 🧠 Foundations of Data Science — NumPy, Pandas & Binary Classification

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:0D1117,50:1F6FEB,100:58A6FF&height=120&text=Foundations%20of%20Data%20Science&fontSize=30&fontColor=ffffff&animation=fadeIn" width="100%"/>

![Python](https://img.shields.io/badge/Python-3.x-blue?logo=python&logoColor=white)
![NumPy](https://img.shields.io/badge/NumPy-1.x-013243?logo=numpy&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-2.x-150458?logo=pandas&logoColor=white)
![Scikit-Learn](https://img.shields.io/badge/Scikit--Learn-1.x-F7931E?logo=scikit-learn&logoColor=white)
![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-orange?logo=jupyter&logoColor=white)
![Colab](https://img.shields.io/badge/Google%20Colab-Ready-F9AB00?logo=googlecolab&logoColor=white)
![License](https://img.shields.io/badge/License-MIT-green?logo=opensourceinitiative)
![Status](https://img.shields.io/badge/Status-Complete-brightgreen)
![Author](https://img.shields.io/badge/Author-MH--SHUVO20-blueviolet?logo=github)

> **A comprehensive, hands-on project covering the core foundations of Data Science using Python.** This notebook walks through numerical computing with NumPy, data manipulation with Pandas, and binary classification evaluation using Scikit-learn — with all actual code, real outputs, and detailed explanations.

---

## 📋 Table of Contents

- [👤 Project Owner & Author](#-project-owner--author)
- [📌 Project Overview](#-project-overview)
- [📁 Project Structure](#-project-structure)
- [📦 Libraries Used](#-libraries-used)
- [🔢 Part 1 — NumPy: Numerical Computing](#-part-1--numpy-numerical-computing)
  - [Task 1 — Array Creation and Operations](#task-1--array-creation-and-operations)
  - [Task 2 — Broadcasting and Reshaping](#task-2--broadcasting-and-reshaping)
- [🐼 Part 2 — Pandas: Data Manipulation](#-part-2--pandas-data-manipulation)
  - [Task 3 — Working with DataFrames](#task-3--working-with-dataframes)
  - [Task 4 — Data Cleaning & Analysis](#task-4--data-cleaning--analysis)
- [🤖 Part 3 — Binary Classification & Evaluation](#-part-3--binary-classification--evaluation)
  - [Task 5 — Dataset-Based Classification Evaluation](#task-5--dataset-based-classification-evaluation)
- [📊 Results Summary](#-results-summary)
- [🚀 Getting Started](#-getting-started)
- [📜 License](#-license)
- [✍️ Author](#️-author)

---

## 👤 Project Owner & Author

<table align="center">
  <tr>
    <td align="center">
      <a href="https://github.com/MH-SHUVO20">
        <img src="https://github.com/MH-SHUVO20.png" width="110px;" style="border-radius:50%;border:3px solid #1F6FEB;" alt="MH-SHUVO20"/>
        <br/>
        <sub><b>MD. MEHEDI HASAN SHUVO</b></sub>
      </a>
    </td>
  </tr>
</table>

<p align="center">
  <a href="https://github.com/MH-SHUVO20">
    <img src="https://img.shields.io/badge/GitHub-MH--SHUVO20-181717?style=for-the-badge&logo=github" />
  </a>
  &nbsp;
  <img src="https://komarev.com/ghpvc/?username=MH-SHUVO20&style=for-the-badge&color=1F6FEB" />
</p>

> 💡 **This project was fully designed, developed, and owned by [MD. MEHEDI HASAN SHUVO](https://github.com/MH-SHUVO20).**

---

## 📌 Project Overview

This project builds a strong practical foundation in Data Science by exploring three major pillars:

| 🔢 Pillar | 📚 Library | 🧩 Key Concepts |
|---|---|---|
| **Numerical Computing** | NumPy | Arrays, Broadcasting, Reshaping, Statistics |
| **Data Manipulation** | Pandas | DataFrames, Cleaning, GroupBy, Analysis |
| **Machine Learning** | Scikit-learn | Logistic Regression, Confusion Matrix, Evaluation Metrics |

**Objective:** Build end-to-end data science skills — from raw array manipulation and data cleaning to training a classifier and evaluating it with real metrics.

---

## 📁 Project Structure

```
Foundations-of-Data-Science/
│
├── Foundations_of_Data_Science_NumPy,_Pandas_&_Binary_Classification.ipynb
├── DataFrame.csv           # Output CSV exported from Task 3
└── README.md
```

---

## 📦 Libraries Used

| Library | Version | Purpose |
|---|---|---|
| `numpy` | 1.x+ | Numerical arrays, math operations, broadcasting |
| `pandas` | 2.x+ | DataFrames, CSV loading/exporting, data cleaning |
| `matplotlib` | 3.x+ | Data visualization |
| `seaborn` | 0.x+ | Statistical data visualization |
| `scikit-learn` | 1.x+ | Logistic Regression, confusion matrix, metrics |

---

## 🔢 Part 1 — NumPy: Numerical Computing

### Task 1 — Array Creation and Operations

Three types of arrays were created and operated on:

**Arrays Created:**

| Array Type | Details |
|---|---|
| **1D Array** | Integers from 0 to 20 using `np.arange(0, 21)` |
| **2D Array** | Shape `(4, 5)` with random integers from 10–99 using `np.random.randint(10, 100, size=(4,5))` |
| **Identity Matrix** | 3×3 using `np.eye(3)` |

**Code:**
```python
import numpy as np

# 1D array
OneD_array = np.arange(0, 21)

# 2D array (4x5) with random integers
TwoD_array = np.random.randint(10, 100, size=(4, 5))

# 3x3 identity matrix
identity_matrix = np.eye(3)
```

**Actual Outputs:**
```
1D array of integers from 0 to 20:
[ 0  1  2  3  4  5  6  7  8  9 10 11 12 13 14 15 16 17 18 19 20]

2D array (4x5):
[[39 16 44 45 28]
 [89 65 93 91 32]
 [89 94 55 26 17]
 [71 24 90 49 69]]

3x3 Identity Matrix:
[[1. 0. 0.]
 [0. 1. 0.]
 [0. 0. 1.]]
```

**Statistical Operations on 2D Array:**

```python
mean   = np.mean(TwoD_array)     # → 56.3
median = np.median(TwoD_array)   # → 52.0
std    = np.std(TwoD_array)      # → 27.25
```

| Metric | Value |
|---|---|
| **Mean** | 56.3 |
| **Median** | 52.0 |
| **Standard Deviation** | 27.25 |

**Slicing & Element-wise Multiplication:**
```python
second_row = TwoD_array[1, :]   # → [89 65 93 91 32]
third_col  = TwoD_array[:, 2]   # → [44 93 55 90]

# Element-wise multiplication (reshaped 1D × 2D)
reshaped_OneD = OneD_array[:20].reshape(4, 5)
result = TwoD_array * reshaped_OneD
```

```
Element-wise multiplication result:
[[   0   16   88  135  112]
 [ 445  390  651  728  288]
 [ 890 1034  660  338  238]
 [1065  384 1530  882 1311]]
```

---

### Task 2 — Broadcasting and Reshaping

```python
One_D_arr = np.arange(16)

# Reshape 1D (16,) → 2D (4x4)
newshape_1d = One_D_arr.reshape(4, 4)

# Broadcasting: add [1,2,3,4] to each row
add = newshape_1d + np.array([1, 2, 3, 4])

# Flatten back to 1D
flat = add.flatten()
```

**Outputs:**

```
Reshaped 4x4 Matrix:
[[ 0  1  2  3]
 [ 4  5  6  7]
 [ 8  9 10 11]
 [12 13 14 15]]

After Broadcasting (+ [1,2,3,4] to each row):
[[ 1  3  5  7]
 [ 5  7  9 11]
 [ 9 11 13 15]
 [13 15 17 19]]

Flattened Back to 1D:
[ 1  3  5  7  5  7  9 11  9 11 13 15 13 15 17 19]
```

---

## 🐼 Part 2 — Pandas: Data Manipulation

### Task 3 — Working with DataFrames

A custom employee DataFrame was created with 5 records:

```python
Data = {
    "Name":       ["Alice", "Bob", "Charlie", "Diana", "Evan"],
    "Age":        [25, 30, 28, 35, 40],
    "Department": ["IT", "HR", "IT", "Marketing", "HR"],
    "Salary":     [50000, 45000, 72000, 58000, 60000]
}
df = pd.DataFrame(Data)
```

**Original DataFrame:**

| Name | Age | Department | Salary |
|---|---|---|---|
| Alice | 25 | IT | 50000 |
| Bob | 30 | HR | 45000 |
| Charlie | 28 | IT | 72000 |
| Diana | 35 | Marketing | 58000 |
| Evan | 40 | HR | 60000 |

**Operations Performed:**

1. **Bonus Column** (10% of Salary):

```python
df["Bonus"] = df["Salary"] * 0.10
```

| Name | Age | Department | Salary | Bonus |
|---|---|---|---|---|
| Alice | 25 | IT | 50000 | 5000.0 |
| Bob | 30 | HR | 45000 | 4500.0 |
| Charlie | 28 | IT | 72000 | 7200.0 |
| Diana | 35 | Marketing | 58000 | 5800.0 |
| Evan | 40 | HR | 60000 | 6000.0 |

2. **HR Employees Filter:**

```python
hr_employees = df[df["Department"] == "HR"]
```

| Name | Age | Department | Salary | Bonus |
|---|---|---|---|---|
| Bob | 30 | HR | 45000 | 4500.0 |
| Evan | 40 | HR | 60000 | 6000.0 |

3. **Average Salary by Department:**

```python
avg_salary = df.groupby("Department")["Salary"].mean().reset_index()
```

| Department | Average Salary |
|---|---|
| HR | 52,500 |
| IT | 61,000 |
| Marketing | 58,000 |

4. **Exported to CSV:**

```python
df.to_csv("DataFrame.csv", index=False)
```

---

### Task 4 — Data Cleaning & Analysis

**Dataset:** Medical Insurance dataset loaded directly from a public URL.

```python
url = "https://raw.githubusercontent.com/stedy/Machine-Learning-with-R-datasets/master/insurance.csv"
my_data = pd.read_csv(url)
```

**Dataset Overview:**

| Property | Value |
|---|---|
| **Records** | 1,338 rows |
| **Features** | 7 columns |
| **Missing Values** | ✅ None (0 missing in all columns) |

**Columns & Data Types:**

| Column | Type |
|---|---|
| `age` | int64 |
| `sex` | object |
| `bmi` | float64 |
| `children` | int64 |
| `smoker` | object |
| `region` | object |
| `charges` | float64 |

**First 5 Rows (Sample):**

| age | sex | bmi | children | smoker | region | charges |
|---|---|---|---|---|---|---|
| 19 | female | 27.900 | 0 | yes | southwest | 16884.924 |
| 18 | male | 33.770 | 1 | no | southeast | 1725.552 |
| 28 | male | 33.000 | 3 | no | southeast | 4449.462 |
| 33 | male | 22.705 | 0 | no | northwest | 21984.471 |
| 32 | male | 28.880 | 0 | no | northwest | 3866.855 |

**Descriptive Statistics (`.describe()`):**

| Stat | age | bmi | children | charges |
|---|---|---|---|---|
| count | 1338 | 1338 | 1338 | 1338 |
| mean | 39.21 | 30.66 | 1.09 | 13270.42 |
| std | 14.05 | 6.10 | 1.21 | 12110.01 |
| min | 18 | 15.96 | 0 | 1121.87 |
| 25% | 27 | 26.30 | 0 | 4740.29 |
| 50% | 39 | 30.40 | 1 | 9382.03 |
| 75% | 51 | 34.69 | 2 | 16639.91 |
| max | 64 | 53.13 | 5 | 63770.43 |
|
> **Note:** This dataset had **no missing values** in any column, so no imputation or dropping was required.

---

## 🤖 Part 3 — Binary Classification & Evaluation

### Task 5 — Dataset-Based Classification Evaluation

**Dataset:** Iris dataset (built-in from Scikit-learn), converted to binary classification:

- **Class 1** → Versicolor
- **Class 0** → Not Versicolor (Setosa or Virginica)

**Code:**
```python
from sklearn.datasets import load_iris
from sklearn.linear_model import LogisticRegression
from sklearn.model_selection import train_test_split
from sklearn.metrics import confusion_matrix, accuracy_score, precision_score, recall_score, f1_score

iris = load_iris()
df = pd.DataFrame(iris.data, columns=iris.feature_names)
df['target'] = iris.target
df['binary_target'] = (df['target'] == 1).astype(int)  # 1=Versicolor, 0=Not

X = df[iris.feature_names]
y = df['binary_target']

# Train/Test split: 70% train, 30% test
X_train, X_test, y_train, y_test = train_test_split(X, y, test_size=0.3, random_state=42)

# Train Logistic Regression
model = LogisticRegression()
model.fit(X_train, y_train)

# Predict
y_pred = model.predict(X_test)
```

**Confusion Matrix Output:**

|  | Predicted Negative (0) | Predicted Positive (1) |
|---|---|---|
| **Actual Negative (0)** | TN = 29 | FP = 3 |
| **Actual Positive (1)** | FN = 9 | TP = 4 |

**Confusion Matrix Explained:**

| Term | Value | Meaning |
|---|---|---|
| **True Positive (TP)** | 4 | Correctly predicted Versicolor as Versicolor |
| **True Negative (TN)** | 29 | Correctly predicted Not Versicolor as Not Versicolor |
| **False Positive (FP)** | 3 | Predicted Versicolor, but was actually Not Versicolor |
| **False Negative (FN)** | 9 | Predicted Not Versicolor, but was actually Versicolor |

**Evaluation Metrics:**

| Metric | Value | Interpretation |
|---|---|---|
| **Accuracy** | 0.733 | ~73% of all predictions were correct |
| **Precision** | 0.571 | ~57% of positive predictions were truly Versicolor |
| **Recall** | 0.308 | Model identified only ~31% of actual Versicolor samples |
| **F1-Score** | 0.400 | Moderate balance between precision and recall |

> **Analysis:** The model performs reasonably in overall accuracy (~73%) but has a low recall (30.8%), meaning it misses a significant number of true Versicolor flowers. This is typical in imbalanced binary classification scenarios — the model tends to favor the majority class (Not Versicolor). The F1-score of 0.4 reflects this moderate overall performance.

---

## 📊 Results Summary

| Part | Task | Key Result |
|---|---|---|
| NumPy | Array Creation | 1D (0–20), 2D (4×5), 3×3 Identity Matrix ✅ |
| NumPy | Statistics | Mean=56.3, Median=52.0, Std=27.25 ✅ |
| NumPy | Broadcasting | Reshape (16→4×4), Add row-wise, Flatten ✅ |
| Pandas | DataFrame | 5-employee DF with Bonus column & CSV export ✅ |
| Pandas | Data Cleaning | 1,338-row insurance dataset, 0 missing values ✅ |
| ML | Classification | Logistic Regression on Iris (binary), Accuracy=73.3% ✅ |

---

## 🚀 Getting Started

### Prerequisites

Make sure you have Python 3.x installed. Install the required libraries:

```bash
pip install numpy pandas matplotlib seaborn scikit-learn
```

### Run Locally

```bash
# Clone the repository
git clone https://github.com/MH-SHUVO20/Foundations-of-Data-Science.git
cd Foundations-of-Data-Science

# Open in Jupyter
jupyter notebook "Foundations_of_Data_Science_NumPy,_Pandas_&_Binary_Classification.ipynb"
```

### Run on Google Colab

Click below to open directly in Google Colab:

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/MH-SHUVO20/Foundations-of-Data-Science/blob/main/Foundations_of_Data_Science_NumPy%2C_Pandas_%26_Binary_Classification.ipynb)

---

## 📜 License

This project is open-source and available under the [MIT License](https://opensource.org/licenses/MIT).  
Copyright (c) 2025 MD. MEHEDI HASAN SHUVO  
Feel free to use, modify, and distribute it with appropriate attribution.

---

## ✍️ Author

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:0D1117,50:1F6FEB,100:58A6FF&height=130&text=MD.%20MEHEDI%20HASAN%20SHUVO&fontSize=26&fontColor=ffffff&animation=fadeIn" width="100%"/>

<p align="center">
  <a href="https://github.com/MH-SHUVO20">
    <img src="https://github.com/MH-SHUVO20.png" width="110px" style="border-radius:50%;border:3px solid #1F6FEB;" alt="MD. MEHEDI HASAN SHUVO"/>
  </a>
</p>

<h3 align="center">👨‍💻 MD. MEHEDI HASAN SHUVO</h3>

<p align="center">
  <a href="https://github.com/MH-SHUVO20">
    <img src="https://img.shields.io/badge/GitHub-MH--SHUVO20-181717?style=for-the-badge&logo=github" />
  </a>
  &nbsp;
  <img src="https://komarev.com/ghpvc/?username=MH-SHUVO20&style=for-the-badge&color=1F6FEB" />
</p>

<p align="center">
  <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&pause=1000&color=1F6FEB&center=true&vCenter=true&width=600&lines=Data+Science+Enthusiast;NumPy+%7C+Pandas+%7C+Scikit-learn;Project+Owner+%26+Developer;Foundations+of+Data+Science+%E2%80%94+2025" alt="Typing SVG" />
</p>

<table align="center">
  <tr>
    <th>Field</th>
    <th>Details</th>
  </tr>
  <tr>
    <td>🧑 <b>Full Name</b></td>
    <td>MD. MEHEDI HASAN SHUVO</td>
  </tr>
  <tr>
    <td>🐙 <b>GitHub</b></td>
    <td><a href="https://github.com/MH-SHUVO20">@MH-SHUVO20</a></td>
  </tr>
  <tr>
    <td>🎯 <b>Role</b></td>
    <td>Project Creator & Owner</td>
  </tr>
  <tr>
    <td>📁 <b>Repository</b></td>
    <td><a href="https://github.com/MH-SHUVO20/Foundations-of-Data-Science">MH-SHUVO20/Foundations-of-Data-Science</a></td>
  </tr>
  <tr>
    <td>🏷️ <b>Project Type</b></td>
    <td>Data Science / Foundations — NumPy, Pandas, ML</td>
  </tr>
  <tr>
    <td>📅 <b>Year</b></td>
    <td>2025</td>
  </tr>
</table>

<br/>

<p align="center">
  <a href="https://github.com/MH-SHUVO20/Foundations-of-Data-Science">
    <img src="https://github-readme-streak-stats.demolab.com?user=MH-SHUVO20&theme=dark&hide_border=true&border_radius=10" alt="GitHub Streak" />
  </a>
</p>

<br/>

<p align="center"><i>"Data is not just numbers — it's the language of insight."</i></p>

<p align="center">⭐ If you found this project helpful, please consider giving it a <b>star</b>!</p>

<p align="center">Made with ❤️ by <b>MD. MEHEDI HASAN SHUVO</b> — 2025</p>

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:58A6FF,50:1F6FEB,100:0D1117&height=100&section=footer" width="100%"/>