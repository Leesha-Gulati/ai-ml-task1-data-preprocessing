# 🛠️ Task 1 – Data Cleaning & Preprocessing (Titanic Dataset)

Welcome to my submission for **Task 1 of the AI & ML Internship**, where I worked on the Titanic dataset to explore and practice **real-world data preprocessing techniques**. This task was not just about fulfilling the minimum requirements — I took this as a learning opportunity to go deeper, explore beyond the checklist, and truly understand each step.

---

## 🧠 What I Learned

Throughout this task, I focused on *learning by doing*. I researched, experimented, and debugged everything myself instead of just following tutorials blindly. Here’s what I learned in detail:

### 🔹 Understanding the Data
- Explored data types (`int`, `float`, `object`)
- Used `.info()`, `.describe()`, `.isnull()` to understand structure and missing values
- Identified columns that needed special handling (like `'Cabin'`, `'Embarked'`, `'Age'`)

### 🔹 Handling Missing Values
- Replaced missing `Age` values with the **median** (better for skewed distributions)
- Filled missing `Embarked` entries using the **mode**
- Dropped the `Cabin` column as it had over 77% missing values

### 🔹 Categorical Variable Encoding
- Converted `Sex` to numeric (male → 0, female → 1)
- One-hot encoded `Embarked` to avoid dummy variable trap
- Extracted **Title** from `Name` (Mr, Miss, Mrs, etc.) and encoded it after grouping rare titles

### 🔹 Feature Engineering (Extra Step)
I went beyond the basic task by:
- Extracting `Title` from the `Name` column to uncover social insights
- Creating a new feature called `FamilySize` (SibSp + Parch + 1)

### 🔹 Feature Scaling
- Standardized `Age` and `Fare` using **StandardScaler** from `sklearn`
- Ensured data was normally distributed with mean ≈ 0 and std ≈ 1

### 🔹 Outlier Detection and Removal
- Used **boxplots** and the **IQR (Interquartile Range)** method to identify and remove extreme values from `Age` and `Fare`

---

## 💾 Files in This Repository

| File Name | Description |
|-----------|-------------|
| `task1.ipynb` | Jupyter notebook containing all code, logic, and plots |
| `titanic_final_cleaned.csv` | Final cleaned and preprocessed dataset |
| `README.md` | You're reading it :) |
| (Optional) screenshots/plots | For visual proof if needed |

---

## 📈 Technologies Used

- **Python** (Pandas, NumPy, Matplotlib, Seaborn)
- **Jupyter Notebook**
- **scikit-learn (StandardScaler)**
- GitHub (for version control and submission)

---

## 👩‍💻 Done By Me — With Full Understanding

I want to clearly state that:
> This task was **entirely completed by me — Leesha Gulati** — without copying from others. I took my time to understand each line of code, explored errors, looked up documentation, and learned **how data preprocessing works in real ML pipelines.**

This is more than just a submission; it’s a reflection of my learning journey. 🙌

---

## 📌 Summary of Key Concepts I Now Understand

- Types of missing data (MCAR, MAR, MNAR)
- Encoding methods (Label, One-Hot, Ordinal)
- Standardization vs. Normalization
- Outlier detection using IQR & boxplots
- Why data cleaning directly affects model performance

---

## ✅ Status: Completed

This repository is complete and ready for review.  
I’m excited to continue learning in this internship and improve with every task!



Thank you for reviewing my work!  
— *Leesha Gulati*
