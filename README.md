# 🧺 Orange vs Grapefruit: ML Classification with Decision Trees & Random Forest

An end-to-end machine learning pipeline to classify citrus fruits using physical attributes like weight, diameter, and color score. This project demonstrates the power of **decision trees**, **ensemble learning**, and **hyperparameter tuning** in achieving high classification accuracy.

---

## 📌 Project Overview

The goal is to predict whether a fruit is an **Orange** or **Grapefruit** based on a structured dataset. This project includes all the major steps in a supervised learning workflow—**data cleaning**, **exploratory data analysis**, **model building**, **hyperparameter tuning**, and **performance evaluation**.

---

## 🎯 Objectives

- Preprocess citrus dataset for modeling
- Explore the structure and distribution of fruit features
- Train and compare Decision Tree vs Random Forest classifiers
- Use GridSearchCV for hyperparameter tuning
- Evaluate and visualize model performance

---

## 🗂️ Dataset

Features included:

- **Diameter**  
- **Weight**  
- **Color Score**  
- **Label** (Orange/Grapefruit)

---

## 🔍 Key Highlights of the Project

### ✅ Data Loading & Preprocessing

- Loaded the dataset with structured features  
- Checked for nulls and anomalies using `.info()` and `.describe()`  
- Applied **Label Encoding** to convert fruit types into binary numerical labels  
- Performed **80-20 train-test split** using `train_test_split()`  

### 📊 Exploratory Data Analysis (EDA)

- Visualized class distributions using:
  - Histograms
  - Boxplots
  - Pairplots
- Checked for class separability and feature influence
- Used a custom `Dis_Stats` module to extract statistical feature summaries

### 🤖 Model Building

- Trained a **Decision Tree Classifier** as a baseline model  
- Improved performance with **Random Forest Classifier** — an ensemble method combining multiple decision trees for robustness

### 🔧 Hyperparameter Tuning

- Used **GridSearchCV** to find optimal settings for Random Forest:
  - `n_estimators`
  - `max_depth`
  - `criterion`
- Reduced overfitting and improved cross-validation accuracy

### 📈 Model Evaluation & Comparison

Evaluated both models using:

- ✅ Accuracy Score  
- 📊 Confusion Matrix  
- 📋 Classification Report (Precision, Recall, F1-Score)

**Result:**  
Random Forest outperformed the Decision Tree in both accuracy and generalization, showcasing the benefits of ensemble learning.

---

## 🛠 Tools & Technologies Used

- **Python**
  - `pandas`, `numpy` – data handling
  - `matplotlib`, `seaborn` – data visualization
  - `scikit-learn` – ML modeling, evaluation, tuning
- **GridSearchCV** – hyperparameter optimization
- **Jupyter Notebook** – step-by-step workflow presentation

---

## 💡 Conclusion

This project shows how even simple datasets can benefit from:

- Thoughtful **EDA** and feature exploration  
- Powerful **ensemble models** like Random Forest  
- Systematic **hyperparameter tuning**

In real-world classification problems, selecting the right algorithm and refining it through data-driven tuning is key to robust performance.

---

## 🔮 Future Enhancements

- Visualize individual decision trees in the forest  
- Add feature importance plots  
- Test on imbalanced datasets or multiclass fruit prediction  
- Deploy model using Streamlit or Flask
