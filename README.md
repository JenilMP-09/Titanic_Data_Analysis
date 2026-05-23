# 🚢 Titanic Data Analysis

![Python](https://img.shields.io/badge/Python-3.x-blue?logo=python&logoColor=white)
![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-orange?logo=jupyter&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-Data%20Analysis-150458?logo=pandas&logoColor=white)
![Seaborn](https://img.shields.io/badge/Seaborn-Visualization-4C72B0)
![Status](https://img.shields.io/badge/Status-Complete-brightgreen)

> Exploratory data analysis on the Titanic dataset to uncover survival patterns across gender, passenger class, and age groups — using Python, Pandas, Seaborn, and Matplotlib.

---

## 📋 Table of Contents

- [Overview](#-overview)
- [Dataset](#-dataset)
- [Project Structure](#-project-structure)
- [Installation](#-installation)
- [Usage](#-usage)
- [Analysis & Findings](#-analysis--findings)
- [Visualizations](#-visualizations)
- [Why This Project](#-why-this-project)

---

## 🔍 Overview

This notebook is **Task 2** in a Data Science learning series. Building on data cleaning skills from Task 1 (Student Performance Dataset), this task dives into one of the most well-known datasets in Data Science — the **Titanic Dataset** — to analyze who survived and why.

**Goals:**
- Load and inspect the Titanic dataset
- Handle missing/null values through appropriate imputation strategies
- Answer analytical questions about survival patterns
- Produce clear visualizations to communicate findings

---

## 📦 Dataset

**Source:** [Kaggle — Titanic Dataset](https://www.kaggle.com/c/titanic/data)

| Column     | Description                                      |
|------------|--------------------------------------------------|
| `Survived` | Survival status (1 = Survived, 0 = Did not survive) |
| `Pclass`   | Passenger class (1st, 2nd, 3rd)                  |
| `Sex`      | Gender of the passenger                          |
| `Age`      | Age in years                                     |
| `Fare`     | Ticket fare paid                                 |
| `Cabin`    | Cabin number *(dropped — ~78% missing)*          |

---

## 📁 Project Structure

```
titanic-data-analysis/
│
├── Task_2_Titanic_Data_Analysis.ipynb   # Main Jupyter notebook
└── README.md                            # Project documentation
```

---

## ⚙️ Installation

1. **Clone the repository:**
   ```bash
   git clone https://github.com/your-username/titanic-data-analysis.git
   cd titanic-data-analysis
   ```

2. **Install required libraries:**
   ```bash
   pip install pandas seaborn matplotlib
   ```

3. **Download the dataset** from [Kaggle](https://www.kaggle.com/c/titanic/data) and update the file path in the notebook.

---

## ▶️ Usage

Open the notebook in Jupyter or Google Colab:

```bash
jupyter notebook Task_2_Titanic_Data_Analysis.ipynb
```

Or open directly in **Google Colab** by uploading the `.ipynb` file.

---

## 📊 Analysis & Findings

### 🧹 Data Cleaning

| Column   | Issue                  | Strategy                                  |
|----------|------------------------|-------------------------------------------|
| `Age`    | Missing values         | Filled with **median** (robust to outliers) |
| `Fare`   | Missing values         | Filled with **median**                    |
| `Cabin`  | ~78% missing           | **Dropped** entirely                      |

---

### ❓ Key Questions Answered

**1. Who survived more — males or females?**
- Females had a dramatically higher survival rate compared to males.
- 📌 *Females survived significantly more.*

**2. Did passenger class affect survival chances?**
- Survival rates were calculated per class using `.mean()` on the `Survived` column.
- 📌 *Yes — higher-class passengers had considerably better survival odds.*

**3. What was the survival rate by age group?**

| Age Group        | Age Range |
|------------------|-----------|
| Child            | 0 – 12    |
| Teen             | 13 – 18   |
| Young Adult      | 19 – 30   |
| Adult            | 31 – 45   |
| Middle-aged      | 46 – 60   |
| Senior           | 61 – 80   |

---

## 📈 Visualizations

| Chart | Description |
|-------|-------------|
| Bar Chart | Survival rate by **gender** |
| Bar Chart | Survival rate by **passenger class** |
| Histogram | Distribution of **passenger ages** (with KDE curve) |

All visualizations are generated using **Seaborn** and **Matplotlib**.

---

## 💡 Why This Project

- ✅ Teaches handling of real-world, messy data
- ✅ Introduces data visualization — a core Data Science skill
- ✅ Practices deriving actionable insights from structured datasets
- ✅ Builds familiarity with `pandas`, `seaborn`, and `matplotlib`

---

## 🛠️ Tech Stack

| Tool         | Version  |
|--------------|----------|
| Python       | 3.x      |
| Pandas       | Latest   |
| Seaborn      | Latest   |
| Matplotlib   | Latest   |
| Jupyter      | Latest   |

---

## 📄 License

This project is open-source and available under the [MIT License](LICENSE).

---

*Part of a Data Science learning series — Task 2 of N*
