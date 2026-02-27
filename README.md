# Foundations of Data Science — NumPy, Pandas & Binary Classification

A comprehensive, hands-on project covering the core foundations of Data Science using Python. This notebook walks through numerical computing with NumPy, data manipulation with Pandas, and binary classification evaluation using Scikit-learn.

---

## Table of Contents

- [Overview](#overview)
- [Project Structure](#project-structure)
- [Technologies Used](#technologies-used)
- [Part 1 — NumPy: Numerical Computing](#part-1--numpy-numerical-computing)
- [Part 2 — Pandas: Data Manipulation](#part-2--pandas-data-manipulation)
- [Part 3 — Binary Classification & Evaluation](#part-3--binary-classification--evaluation)
- [Results](#results)
- [Getting Started](#getting-started)

---

## Overview

This project is designed to build a strong practical foundation in Data Science by exploring three major pillars:

| Pillar | Library | Key Concepts |
|---|---|---|
| Numerical Computing | NumPy | Arrays, Broadcasting, Reshaping |
| Data Manipulation | Pandas | DataFrames, Cleaning, Analysis |
| Machine Learning | Scikit-learn | Classification, Confusion Matrix, Metrics |

---

## Project Structure

```
Foundations of Data Science/
│
├── Foundations_of_Data_Science_NumPy,_Pandas_&_Binary_Classification.ipynb
├── DataFrame.csv           # Output CSV from Task 3
└── README.md
```

---

## Technologies Used

- **Python 3.x**
- **NumPy** — Array operations and numerical computing
- **Pandas** — Data loading, cleaning, and analysis
- **Matplotlib / Seaborn** — Data visualization
- **Scikit-learn** — Machine learning model and evaluation metrics

---

## Part 1 — NumPy: Numerical Computing

### Task 1: Array Creation and Operations
- Created a **1D array** of integers from 0 to 20
- Created a **2D array** of shape `(4, 5)` with random integers from 10 to 99
- Created a **3×3 identity matrix**
- Computed **mean, median, and standard deviation** of the 2D array
- Performed **row/column slicing** and **element-wise multiplication**

### Task 2: Broadcasting and Reshaping
- Reshaped a 1D array of size 16 into a **4×4 matrix**
- Applied **broadcasting** to add `[1, 2, 3, 4]` to each row
- Flattened the matrix back to a **1D array**

---

## Part 2 — Pandas: Data Manipulation

### Task 3: Working with DataFrames
- Built a custom DataFrame with columns: `Name`, `Age`, `Department`, `Salary`
- Added a derived column: **Bonus** (10% of Salary)
- Filtered employees by **department (HR)**
- Calculated **average salary per department** using `groupby()`
- Exported the DataFrame to **`DataFrame.csv`**

### Task 4: Data Cleaning & Analysis
- Loaded the **Medical Insurance dataset** from a public GitHub source
- Explored dataset:
  - First/Last 5 rows
  - Shape, columns, and data types
- Checked for **missing values** (dataset had none)
- Generated **descriptive statistics** using `.describe()`

> Dataset Source: [Machine Learning with R Datasets — Insurance.csv](https://raw.githubusercontent.com/stedy/Machine-Learning-with-R-datasets/master/insurance.csv)

---

## Part 3 — Binary Classification & Evaluation

### Task 5: Dataset-Based Classification Evaluation

Using the **Iris dataset**, the problem was converted into a **binary classification** task:
- **Class 1** → Versicolor
- **Class 0** → Not Versicolor

**Steps:**
1. Split data: **70% training / 30% testing**
2. Trained a **Logistic Regression** classifier
3. Predicted on the test set
4. Generated the **Confusion Matrix**

### Confusion Matrix Results

|  | Predicted Negative | Predicted Positive |
|---|---|---|
| **Actual Negative** | TN = 29 | FP = 3 |
| **Actual Positive** | FN = 9 | TP = 4 |

### Evaluation Metrics

| Metric | Value | Interpretation |
|---|---|---|
| **Accuracy** | 0.733 | ~73% of all predictions were correct |
| **Precision** | 0.571 | ~57% of positive predictions were truly positive |
| **Recall** | 0.308 | Model identified ~31% of actual Versicolor samples |
| **F1-Score** | 0.400 | Moderate balance between precision and recall |

> The model performs reasonably on overall accuracy but has lower recall, indicating it misses a notable number of true Versicolor flowers. This is typical in imbalanced binary classification scenarios.

---

## Getting Started

### Prerequisites

Ensure you have Python 3.x installed along with the following packages:

```bash
pip install numpy pandas matplotlib seaborn scikit-learn
```

### Run the Notebook

1. Clone or download this repository
2. Open the notebook in **VS Code**, **Jupyter Lab**, or **Google Colab**
3. Run all cells sequentially from top to bottom

```bash
jupyter notebook "Foundations_of_Data_Science_NumPy,_Pandas_&_Binary_Classification.ipynb"
```

---

## License

This project is open-source and available under the [MIT License](https://opensource.org/licenses/MIT).  
Feel free to use, modify, and distribute it with appropriate attribution.
