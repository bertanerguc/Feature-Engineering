# 🌟 Diabetes Feature Engineering

This project involves building a machine learning model to predict whether a person has diabetes based on their medical data. The focus is on applying **feature engineering** techniques and preparing the dataset for modeling.

---

## 🚀 Project Overview

### 📝 Problem Statement
The objective is to develop a predictive model using machine learning to determine if an individual is diabetic. The dataset includes features from a diabetes study conducted on Pima Indian women aged 21 and above in Phoenix, Arizona.

### 📊 Dataset
The dataset consists of **768 observations** and **8 numerical features**, along with a binary target variable indicating diabetes status:
- **Outcome**: 1 (diabetic) or 0 (non-diabetic).

---

## 📂 Dataset Features

| Feature                      | Description                                                 |
|------------------------------|-------------------------------------------------------------|
| `Pregnancies`                | Number of pregnancies                                       |
| `Glucose`                    | Plasma glucose concentration                                |
| `BloodPressure`              | Diastolic blood pressure (mm Hg)                           |
| `SkinThickness`              | Triceps skin fold thickness (mm)                           |
| `Insulin`                    | 2-Hour serum insulin (mu U/ml)                             |
| `BMI`                        | Body mass index (weight in kg/(height in m)^2)             |
| `DiabetesPedigreeFunction`   | Diabetes pedigree function                                 |
| `Age`                        | Age in years                                               |
| `Outcome`                    | Diabetes test result (1 = Positive, 0 = Negative)          |

---

## 🔧 Key Features

### 🛠 Tasks

1. **Exploratory Data Analysis (EDA)**:
   - Analyze numerical and categorical variables.
   - Handle missing values and outliers.
   - Perform correlation analysis.
2. **Feature Engineering**:
   - Address missing and incorrect values.
   - Create new meaningful features.
   - Standardize numerical features.
3. **Modeling**:
   - Train a **Random Forest Classifier** to predict diabetes.
   - Evaluate the model using metrics such as accuracy, recall, precision, F1 score, and ROC-AUC.

---

## 📈 Project Workflow

### 1️⃣ Data Understanding and Preparation
- Perform EDA to understand data distribution and relationships.
- Handle missing and outlier values effectively.

### 2️⃣ Feature Engineering
- Replace zero values in features like `Glucose`, `Insulin`, and `BMI` with NaN, then impute with medians.
- Create new features such as:
  - **Age categories** (e.g., `mature`, `senior`).
  - **BMI categories** (e.g., `underweight`, `obese`).
  - Interaction terms (e.g., `Glucose * Insulin`).

### 3️⃣ Encoding and Standardization
- Apply **label encoding** for binary categorical features.
- Use **one-hot encoding** for multi-class categorical features.
- Standardize numerical features for better model performance.

### 4️⃣ Modeling
- Train a **Random Forest Classifier** using the processed data.
- Evaluate the model using performance metrics.

---

## 📊 Results

### 🎯 Performance Metrics

| Metric         | Value |
|----------------|-------|
| **Accuracy**   | 0.79  |
| **Recall**     | 0.71  |
| **Precision**  | 0.67  |
| **F1 Score**   | 0.69  |
| **ROC-AUC**    | 0.77  |

### 🛠 Feature Importance
Key features contributing to model predictions include:
- Glucose
- BMI
- Age
- Diabetes Pedigree Function

![Feature Importance](importances.png)

---

## 🛠 Tools and Libraries

- **Python**  
- **Pandas**  
- **NumPy**  
- **Matplotlib**  
- **Seaborn**  
- **Scikit-learn**  

---

## 🌟 Contribution

Contributions are welcome!  
Feel free to fork this repository, create issues, or submit pull requests for improvements.

---

## 📜 License

This project is licensed under the [MIT License](LICENSE).

