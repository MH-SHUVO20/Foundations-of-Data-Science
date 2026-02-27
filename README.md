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

> **A comprehensive, hands-on project covering the core foundations of Data Science using Python.** This notebook walks through numerical computing with NumPy, data manipulation with Pandas, and binary classification evaluation using Scikit-learn — with real outputs and detailed explanations.

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
├── LICENSE
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

> **Goal:** Create different types of NumPy arrays and perform statistical and element-wise operations on them.

**What was done:**

- Created a **1D array** of integers ranging from 0 to 20 using `np.arange()`
- Created a **2D array** of shape `(4×5)` filled with random integers between 10 and 99
- Created a **3×3 Identity Matrix** using `np.eye()`
- Computed key **statistical metrics** on the 2D array: Mean, Median, and Standard Deviation
- Performed **array slicing** to extract the second row and third column
- Applied **element-wise multiplication** between the reshaped 1D array and the 2D array

**Key Results:**

| Metric | Value |
|---|---|
| **Mean** | 56.3 |
| **Median** | 52.0 |
| **Standard Deviation** | 27.25 |

---

### Task 2 — Broadcasting and Reshaping

> **Goal:** Demonstrate NumPy's broadcasting capability and array reshaping techniques.

**What was done:**

- Created a 1D array of 16 elements and **reshaped** it into a `(4×4)` 2D matrix
- Applied **broadcasting** by adding a 1D vector `[1, 2, 3, 4]` to every row of the matrix simultaneously — without any loops
- **Flattened** the resulting 2D matrix back into a 1D array

**Key Insight:** Broadcasting allows operations between arrays of different shapes without copying data, making computations both memory-efficient and fast.

---

## 🐼 Part 2 — Pandas: Data Manipulation

### Task 3 — Working with DataFrames

> **Goal:** Build a custom DataFrame, perform transformations, filter data, and export it.

**What was done:**

- Manually created a **5-record employee DataFrame** with columns: Name, Age, Department, Salary
- Added a new **Bonus column** calculated as 10% of each employee's Salary
- **Filtered** the DataFrame to extract only HR department employees
- Calculated the **average salary per department** using `groupby()`
- **Exported** the final DataFrame to a CSV file (`DataFrame.csv`)

**Department-wise Average Salary:**

| Department | Average Salary |
|---|---|
| HR | 52,500 |
| IT | 61,000 |
| Marketing | 58,000 |

---

### Task 4 — Data Cleaning & Analysis

> **Goal:** Load a real-world dataset, inspect its quality, handle missing values, and extract statistical insights.

**Dataset Used:** Medical Insurance dataset (loaded directly from a public URL — no manual download needed)

**What was done:**

- Loaded the dataset directly from a remote URL using `pd.read_csv()`
- Inspected the **shape, column names, and data types** of all 7 features
- Checked for **missing values** across all columns
- Generated **descriptive statistics** (mean, std, min, max, quartiles) using `.describe()`
- Analyzed the **distribution** of numerical features like age, BMI, and charges

**Dataset Overview:**

| Property | Value |
|---|---|
| **Records** | 1,338 rows |
| **Features** | 7 columns (age, sex, bmi, children, smoker, region, charges) |
| **Missing Values** | ✅ None — dataset was clean, no imputation needed |
| **Average Charges** | $13,270.42 |
| **Age Range** | 18 – 64 years |
| **BMI Range** | 15.96 – 53.13 |

---

## 🤖 Part 3 — Binary Classification & Evaluation

### Task 5 — Dataset-Based Classification Evaluation

> **Goal:** Train a binary classifier on a real dataset and evaluate its performance using standard ML metrics.

**Dataset Used:** Iris dataset (built-in from Scikit-learn), converted to a binary problem:
- **Class 1** → Versicolor
- **Class 0** → Not Versicolor (Setosa or Virginica)

**What was done:**

- Loaded the Iris dataset and **converted it to a binary classification** problem
- Split data into **70% training / 30% testing** sets using `train_test_split()`
- Trained a **Logistic Regression** model on the training set
- Generated **predictions** on the test set
- Built and interpreted a full **Confusion Matrix**
- Computed all standard **evaluation metrics**: Accuracy, Precision, Recall, F1-Score

**Confusion Matrix:**

|  | Predicted Negative (0) | Predicted Positive (1) |
|---|---|---|
| **Actual Negative (0)** | TN = 29 | FP = 3 |
| **Actual Positive (1)** | FN = 9 | TP = 4 |

**Evaluation Metrics:**

| Metric | Value | Interpretation |
|---|---|---|
| **Accuracy** | 0.733 | ~73% of all predictions were correct |
| **Precision** | 0.571 | ~57% of predicted Versicolor were truly Versicolor |
| **Recall** | 0.308 | Model detected only ~31% of all actual Versicolor samples |
| **F1-Score** | 0.400 | Moderate balance — model struggled with the minority class |

> **Analysis:** The model achieves reasonable overall accuracy (~73%) but has a low recall (30.8%), indicating it misses many true Versicolor instances. This is a classic imbalanced classification scenario where the model favors the majority class. The F1-score of 0.4 reflects this trade-off.

---

## 📊 Results Summary

| Part | Task | Key Result |
|---|---|---|
| NumPy | Array Creation & Stats | 1D, 2D, Identity Matrix — Mean=56.3, Std=27.25 ✅ |
| NumPy | Broadcasting & Reshape | Reshaped (16→4×4), Row-wise broadcast, Flattened ✅ |
| Pandas | DataFrame Operations | 5-employee DF, Bonus column, GroupBy, CSV export ✅ |
| Pandas | Data Cleaning | 1,338-row insurance dataset — 0 missing values ✅ |
| ML | Binary Classification | Logistic Regression on Iris — Accuracy = 73.3% ✅ |

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

This project is open-source and available under the [MIT License](LICENSE).
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
  <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&pause=800&color=58A6FF&center=true&vCenter=true&width=600&lines=Thanks+for+visiting!;Feel+free+to+star+%E2%AD%90+this+repo!;MD.+MEHEDI+HASAN+SHUVO+%E2%80%94+2025" alt="Footer Typing SVG" />
</p>

<p align="center"><i>"Data is not just numbers — it's the language of insight."</i></p>

<p align="center">⭐ If you found this project helpful, please consider giving it a <b>star</b>!</p>

<p align="center">Made with ❤️ by <b>MD. MEHEDI HASAN SHUVO</b> — 2025</p>

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:58A6FF,50:1F6FEB,100:0D1117&height=100&section=footer" width="100%"/>