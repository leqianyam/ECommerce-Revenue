# 🛒 Online Shoppers Intention Analysis

This project analyzes the **Online Shoppers Intention** dataset using Python. It focuses on uncovering patterns behind users’ purchasing decisions through visualizations, correlation analysis, and machine learning.

## 📌 Project Overview

We explore how session-based web data—like page duration, bounce rates, and visitor type—affects a customer's likelihood of purchasing. The project includes:

- Data cleaning & preprocessing
- Exploratory data analysis (EDA)
- Visualizations (histograms, heatmaps, boxplots, violin plots)
- Logistic regression modeling
- Model evaluation using accuracy, confusion matrix, and ROC curve

---

## 📂 Table of Contents

- [Dataset](#dataset)
- [Data Cleaning and Preprocessing](#data-cleaning-and-preprocessing)
- [Exploratory Data Analysis](#exploratory-data-analysis)
- [Correlation and Heatmap](#correlation-and-heatmap)
- [Visualizations](#visualizations)
- [Prediction Model](#prediction-model)
- [Model Evaluation](#model-evaluation)
- [Conclusion](#conclusion)
- [Technologies Used](#technologies-used)

---

## 📊 Dataset

- **Name:** Online Shoppers Purchasing Intention
- **Source:** UCI / Kaggle
- **Records:** 12,330 unique sessions
- **License:** CC BY 4.0

Each record represents a different visitor’s web session, avoiding user- or campaign-specific bias.

---

## 🧹 Data Cleaning and Preprocessing

- Converted object types to appropriate numeric/boolean types.
- Removed or filled missing values.
- Verified data type consistency.
- Categorical columns were label-encoded or one-hot encoded.
- Boolean values were cast as integers to be model-ready.

---

## 📈 Exploratory Data Analysis

Descriptive statistics and initial visualizations (count plots, histograms) helped identify patterns in:

- Bounce & exit rates
- Revenue by visitor type
- Page values & durations

---

## 🔥 Correlation and Heatmap

- Created correlation matrix on numeric features.
- Visualized with `seaborn.heatmap()` to identify multicollinearity and strong relationships.
- Filtered top 5-7 most correlated features with the target variable.

---

## 📊 Visualizations

Used various `matplotlib` and `seaborn` plots:

- **Histograms:** to understand feature distributions
- **Boxplots:** for comparing brand-level metrics (in related projects)
- **Violin plots:** to observe revenue spread across visitor types
- **Bar charts and count plots:** to analyze categorical breakdowns

---

## 🤖 Prediction Model

Used **Logistic Regression** to predict whether a visitor session will lead to revenue:

- Features: page durations, value metrics, user types
- Target: Revenue (binary)
- Data scaled with `StandardScaler`
- Split 80% test / 20% train using `train_test_split`

---

## 📊 Model Evaluation

- **Accuracy score** for model performance
- **Confusion matrix** for visualizing prediction outcomes
- **ROC Curve** with AUC to assess trade-off between TPR and FPR

---

## 🧠 Conclusion

This notebook explored and modeled the Online Shoppers Intention dataset. After preprocessing and visualization, a baseline logistic regression model was implemented. Despite limitations, it offered insight into which web session metrics influence purchasing behavior.

---

## 🛠 Technologies Used

- Python 3.11
- Pandas
- NumPy
- Seaborn
- Matplotlib
- Scikit-learn
- Jupyter Notebook

---

## 📁 How to Run

1. Clone the repo:
   ```bash
   git clone https://github.com/yourusername/online-shoppers-intention.git
   cd online-shoppers-intention

