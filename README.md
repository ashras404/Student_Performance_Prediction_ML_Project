# 🎓 Student Performance Prediction System
### **Machine Learning Pipeline | Regression Analysis**

---

## 📌 Project Overview
This project focuses on building a high-precision predictive model to estimate a student's **Performance Index**. By utilizing a dataset of 10,000 records, the system analyzes academic habits and lifestyle choices to forecast results with industry-leading accuracy.

## 🚀 Final Results
* **Model Accuracy (R² Score):** `0.9890`
* **Success Percentage:** `98.90%`
* **Primary Predictors:** Previous Scores & Hours Studied

---

## 🛠️ Tech Stack & Tools
* **Language:** Python 3.10+
* **IDE:** Google Colab / Jupyter Notebook
* **Libraries:** * `Pandas`: Data structure and cleaning
    * `Scikit-Learn`: Machine Learning (Linear Regression)
    * `Matplotlib`: Feature impact visualization
    * `NumPy`: Array processing for custom input

---

## 📂 Code Structure (Cell-by-Cell)

### **1. Data Acquisition**
Imports necessary libraries and loads the `Student_Performance.csv`. It includes an initial `df.head()` to verify the data structure.

### **2. Exploratory Data Analysis (EDA)**
Uses `df.info()` and `df.describe()` to audit data health, ensuring there are no missing values (NaN) and understanding the statistical range of student scores.

### **3. Feature Encoding**
Converts categorical text ("Yes/No") into binary numeric values (1/0).
> **Why:** Linear Regression requires numeric input for matrix multiplication.

### **4. Validation Split**
Implementation of the **80/20 Train-Test Split**.
* **Training Set:** 8,000 records (The "Study" Phase)
* **Testing Set:** 2,000 records (The "Exam" Phase)

### **5. Model Training**
Initialization and fitting of the **Linear Regression** algorithm. The model calculates the coefficients (weights) for each feature to find the "Line of Best Fit."

### **6. Evaluation**
Uses the $R^2$ metric to compare predicted values against actual historical values. Our score of **0.9890** indicates a near-perfect correlation.

### **7. Inference Tool**
A custom interaction cell where new data can be entered to receive an instant performance prediction (e.g., Input: 8hrs study -> Prediction: 80.25).

---

## 📈 Key Insights
* **Study Time Correlation:** Every additional hour of study shows a measurable, linear increase in the Performance Index.
* **Socio-Economic Factors:** Previous academic success remains the strongest indicator of future performance according to the model's coefficient weights.

---

**Developed for Presentation at Integral University**
*April 2026*
