# Student Admission Records Analysis

[Dataset Link](https://www.kaggle.com/datasets/zeeshier/student-admission-records)

---

## 📘 Dataset Summary

The **Student Admission Record** dataset contains information about students and the factors that may influence their admission decisions into a university or academic program. The dataset includes demographic details, academic performance, and admission outcomes.  

> **Note:** This is the "dirty" version of the dataset. It contains missing values, inconsistencies, and duplicates, which require cleaning before analysis or modeling.

---

## 📊 Data Description

| Column Name               | Description                                      | Type      | Non-Null Count |
|----------------------------|--------------------------------------------------|----------|----------------|
| Name                       | Full name of the student                          | object   | 147            |
| Age                        | Age of the student                               | float64  | 147            |
| Gender                     | Student gender (Male/Female/Other)              | object   | 147            |
| Admission Test Score       | Score obtained in the admission test            | float64  | 146            |
| High School Percentage     | Percentage/grade obtained in high school        | float64  | 146            |
| City                       | City of residence of the student                 | object   | 147            |
| Admission Status           | Final admission result (Admitted/Rejected) — Target | object | 147            |

**Dataset Overview:**
- Number of rows: 158  
- Number of columns: 7  
- Target variable: `Admission Status`  
- Numerical features: Age, Admission Test Score, High School Percentage  
- Categorical features: Name, Gender, City, Admission Status  

---

## 🛠️ Libraries Used
- pandas, numpy — Data handling and preprocessing  
- seaborn, matplotlib — Data visualization  
- scikit-learn — Label encoding and feature scaling  

---

## 🔹 Data Cleaning and Preprocessing

1. **Handling Missing Values**
   - Numerical columns (`Age`, `Admission Test Score`, `High School Percentage`) were filled with **median values**.
   - Categorical columns (`Name`, `Gender`, `City`, `Admission Status`) were filled with `"None"`.

2. **Removing Duplicates**
   - Duplicate rows were detected and removed from the dataset.

3. **Encoding Categorical Features**
   - All categorical features were **label encoded** to numeric values for analysis and modeling.

4. **Normalizing Numerical Features**
   - All numerical features were **standard scaled** to improve consistency for modeling.

5. **Saving Cleaned Data**
   - The processed dataset was saved as `encoded_student_admission_data.csv` for reproducibility.

---

## 🔹 Exploratory Data Analysis (EDA)

**Numerical Features Insights:**
- **Age:** Typically ranges from late teens to early twenties; can affect admission chances.  
- **Admission Test Score:** Positive correlation expected with Admission Status.  
- **High School Percentage:** Higher percentage likely improves admission probability.  

**Categorical Features Insights:**
- **Gender & City:** Useful for demographic analysis and trend detection.  
- **Admission Status:** Target variable for prediction.  

**Visualizations Conducted:**
- Boxplots for outlier detection (e.g., Age).  
- Histograms for distribution of numerical features (e.g., High School Percentage).  
- Value counts for categorical features to observe distribution patterns.

---

## 🔹 General Insights
- Students with higher **Admission Test Scores** and **High School Percentages** tend to have a higher chance of admission.  
- Encoding and scaling make the dataset ready for machine learning models.  
- This dataset can be used to build **predictive models** for admission outcomes.

---

## 🗂️ Project Workflow
1. Import libraries  
2. Load the dataset  
3. Handle missing values  
4. Remove duplicates  
5. Perform EDA (visualizations & descriptive statistics)  
6. Encode categorical columns  
7. Normalize numerical features  
8. Save processed dataset  

---

## ✅ Conclusion
This project demonstrates **data cleaning, preprocessing, and exploratory data analysis** on a real-world, dirty dataset. It prepares the data for predictive modeling while providing insights into student admission trends.

---


