# Jubilant_Assesment
# 📊 Store Sales Analysis & Prediction + 🤖 Policy Q&A Bot

## 📌 Overview

This repository contains solutions for two assignments:

1. **Store Sales Analysis & Prediction**
2. **Simple Policy Q&A Bot**

The project demonstrates practical applications of **Data Analysis, Machine Learning, and Natural Language Processing (NLP)**.

---

# 🟢 Assignment 1: Store Sales Analysis & Prediction

## 🎯 Objective

* Perform Exploratory Data Analysis (EDA)
* Create time-based features
* Train a prediction model
* Evaluate model performance
* Predict future sales

---

## ⚙️ Approach

### 1. Data Preprocessing

* Loaded dataset (`sales_data.csv`)
* Handled missing values using forward fill
* Converted `Date` column to datetime format

### 2. Exploratory Data Analysis (EDA)

* Sales trend over time
* Promotion vs Non-promotion comparison
* Sales distribution across days of the week

### 3. Feature Engineering

* Created **lag feature (`lag_1`)** to capture previous day sales

### 4. Model Building

* Used **Linear Regression**
* Features used:

  * `lag_1`
  * `Promotion`
  * `DayOfWeek`
* Used **last 30 days as test data**

### 5. Evaluation

* Metric used: **Mean Absolute Error (MAE)**

### 6. Prediction

* Predicted sales for the **next 7 days**

---

## 📊 Key Insights

* Promotions significantly increase sales
* Sales show a stable trend with fluctuations
* Mid-week sales are higher than weekends
* Sales depend on previous day values
* Future sales are expected to remain stable

---

# 🤖 Assignment 2: Simple Policy Q&A Bot

## 🎯 Objective

* Build a Q&A system using policy documents
* Retrieve relevant answers from documents
* Handle both general and specific queries

---

## ⚙️ Approach

### 1. Data Loading

* Loaded policy documents:

  * `leave_policy.txt`
  * `it_policy.txt`
  * `travel_policy.txt`

### 2. Text Processing

* Used **TF-IDF Vectorization** to convert text into numerical format

### 3. Retrieval System

* Used **Cosine Similarity** to find the most relevant document

### 4. Answer Generation

* **General queries** → return full policy
* **Specific queries** → return most relevant sentence

### 5. Fallback

* If no relevant answer found:

  ```
  Information not available in policy documents.
  ```

---

## 💡 Key Insights

* TF-IDF effectively captures important keywords
* Cosine similarity enables efficient retrieval
* Sentence-level responses improve clarity
* System handles both general and specific queries
* Simple NLP techniques work effectively without heavy models

---

# 🛠️ Technologies Used

* Python 🐍
* Pandas
* Matplotlib
* Scikit-learn

---

# 📂 Project Structure

```
├── sales_data.csv
├── leave_policy.txt
├── it_policy.txt
├── travel_policy.txt
├── Assignment_notebook.ipynb
├── Assignment_Report.pdf
└── README.md
```

---

# 🚀 How to Run

1. Clone the repository

```
git clone https://github.com/your-username/your-repo-name.git
```

2. Install dependencies

```
pip install pandas matplotlib scikit-learn
```

3. Run the notebook

```
jupyter notebook
```

---

# ✅ Conclusion

This project demonstrates:

* Data analysis and forecasting using machine learning
* Practical implementation of a simple NLP-based Q&A system

---

# 👤 Author

**Manoj Kumar Saroj**

