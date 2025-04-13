# 🧠 Stroke Risk Prediction

## 📌 Project Overview  
Stroke is a critical health condition and a leading cause of death and long-term disability worldwide. This project focuses on predicting the **risk of stroke** using **machine learning models** based on medical and demographic features.  

Two models were implemented and evaluated:  
- **Decision Tree Classifier**  
- **Random Forest Classifier** (🏆 Best Performing)

---

## 📂 Project Resources  
🔹 **Dataset (CSV File)**: [Download healthcare-dataset-stroke-data.csv](https://github.com/SunnyRao07/stroke-risk-prediction/blob/main/healthcare-dataset-stroke-data.csv)  
🔹 **Project Code (.ipynb)**: [View Jupyter Notebook](https://github.com/SunnyRao07/stroke-risk-prediction/blob/main/Stroke%20Risk%20Prediction%20Code.ipynb)  
🔹 **Project Report (DOCX File)**: [Download Report](https://github.com/SunnyRao07/stroke-risk-prediction/blob/main/Stroke%20Risk%20Prediction%20Report.pdf)  
🔹 **Presentation (PPTX File)**: [Download PPT](https://github.com/SunnyRao07/stroke-risk-prediction/blob/main/Stroke%20Risk%20Predictions%20PPT.pptx)

---

## 🧾 Dataset Overview  
- **Total Records**: 5,110  
- **Target Variable**: `stroke` (1 = Stroke occurred, 0 = No stroke)  
- **Features**:  
  - Demographic: Age, Gender, Marital Status, Residence Type  
  - Clinical: Hypertension, Heart Disease, Glucose Level, BMI  
  - Lifestyle: Smoking Status, Work Type  

📝 **Class Imbalance Notice**: Only ~5% of the data points represent stroke cases, making class balancing necessary.

---

## 🛠 Data Preprocessing  
✔️ **Cleaning & Transformation**:  
- Dropped non-informative `id` column  
- Handled missing values in `bmi` using **median imputation**  
- Encoded categorical variables using `LabelEncoder`  

✔️ **Outlier Removal**:  
- Used **IQR method** to eliminate outliers in `bmi` and `avg_glucose_level`  

✔️ **Feature Scaling**:  
- Applied `StandardScaler` to numerical columns  

✔️ **Train-Test Split**:  
- 80% Training, 20% Testing using **Stratified Sampling**

✔️ **Imbalance Handling**:  
- Used **SMOTE (Synthetic Minority Over-sampling Technique)** on training set

---

## 📊 Exploratory Data Analysis  
- **Visualizations**: Histograms, KDE plots, bar charts, and heatmaps  
- **Findings**:  
  - Higher age and glucose levels correlate positively with stroke risk  
  - Hypertension and heart disease increase likelihood of stroke  
  - Gender and residence type have minimal impact

---

## 🤖 Models Used  

### 1️⃣ **Decision Tree Classifier**  
✔️ Transparent and interpretable  
❌ Slightly lower accuracy on imbalanced data  

### 2️⃣ **Random Forest Classifier** (🏆 Best Model)  
✅ High accuracy and better generalization  
✅ Handles imbalance effectively with SMOTE  
✅ Offers feature importance insights

---

## 📈 Model Performance

| Model           | Accuracy | Precision | F1 Score |
|----------------|----------|-----------|----------|
| Decision Tree  | 89.5%    | 68.2%     | 74.4%    |
| **Random Forest** | **93.7%** | **75.9%**   | **81.1%**  |

📌 **Random Forest** outperformed Decision Tree in all metrics.

---

## 🔍 Feature Importance  
The top predictors identified by the **Random Forest** model:  
- **Age** 🥇  
- **Average Glucose Level**  
- **BMI**  
- **Hypertension**  
- **Heart Disease**  
- **Smoking Status**

---

## 🚀 Future Scope  
🔹 Incorporate more clinical features (blood pressure, cholesterol, medication history)  
🔹 Apply deep learning methods (e.g., Neural Networks, LSTM)  
🔹 Develop a real-time **decision support system** for healthcare providers  

---

## 🏗 Project Highlights  
This project showcases the complete data science workflow for stroke risk prediction, including:  
✔️ Data Preprocessing & Cleaning  
✔️ Exploratory Data Analysis and Feature Engineering  
✔️ Model Development and Evaluation (Decision Tree, Random Forest)  
✔️ Report, Visualization, and Documentation  


---
