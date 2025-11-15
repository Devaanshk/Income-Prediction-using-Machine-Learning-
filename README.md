# Income Prediction Using Machine Learning

This project predicts whether an individual earns **more than \$50K/year** using census and demographic attributes from the **UCI Adult Income Dataset**.  
The workflow includes **exploratory data analysis (EDA)**, **data preprocessing**, **handling class imbalance**, and training **five machine learning models**, followed by a full **performance comparison**.

---

## 🔍 Project Summary

The goal is to build a reliable model that predicts high-income individuals using demographic and employment-related features such as:

- Age  
- Education level  
- Occupation  
- Gender  
- Workclass  
- Marital status  
- Hours-per-week  
- Capital gain/loss  

The dataset is known for its **class imbalance** (majority: `<=50K`), making it ideal for demonstrating real-world ML handling techniques.

---

## 🚀 Models Implemented

This project trains and evaluates **five** different ML models:

1. **Logistic Regression**  
2. **Support Vector Machine (SVM)**  
3. **Random Forest**  
4. **XGBoost Classifier**  
5. **Neural Network (TensorFlow/Keras)**  

Each model is evaluated on:

- **Accuracy**  
- **Sensitivity (Recall for >50K)**  
- **Specificity (Recall for <=50K)**  
- **F1 Score**  
- **Training time**  

---

## 🧠 Key Features

- ✔ Full **EDA with visualizations** (distribution plots, correlation heatmaps, class imbalance).  
- ✔ Custom preprocessing pipelines for numerical and categorical features.  
- ✔ **Label encoding**, **one-hot encoding**, and **standardization**.  
- ✔ **SMOTE** for balancing minority (>50K) class.  
- ✔ Confusion matrices and ROC curves for detailed model insights.  
- ✔ Feature importance plots (Random Forest & XGBoost).  
- ✔ Neural network architecture with dropout layers for regularization.  
- ✔ Final comparison table + ranked model performance.

---

## 📂 Project Structure

income-prediction/
├── train.csv
├── test.csv
├── income_prediction.ipynb or .py
├── README.md
└── (Outputs: plots, comparison tables, etc.)


---

## 🧪 Methodology

### **1. Data Preprocessing**
- Replace `'?'` with `NaN`  
- Detect and handle missing values  
- Encode categorical features using **LabelEncoder** and **OneHotEncoder**  
- Standardize continuous variables using **StandardScaler**  
- Apply **SMOTE** to reduce class imbalance

### **2. Exploratory Data Analysis**
- Income distribution  
- Age distribution by income  
- Gender vs income  
- Education vs income  
- Marital status vs income  
- Correlation heatmaps  

### **3. Model Training**
Each model receives fully preprocessed data with consistent encoding.  
Hyperparameters tuned (Random Forest via GridSearchCV).

### **4. Evaluation Metrics**
For each model:

- Confusion Matrix  
- Accuracy  
- Sensitivity & Specificity  
- ROC Curve (Logistic Regression)  
- Training time summary  
- Top 10 feature importance (RF & XGBoost)

---

## 📊 Results Summary

The models are compared on:

| Model                | Accuracy | Sensitivity (>50K) | Specificity (<=50K) | F1 Score | Notes |
|---------------------|----------|---------------------|----------------------|----------|-------|
| Logistic Regression | —        | —                   | —                    | —        | Baseline model |
| SVM                 | —        | —                   | —                    | —        | Good sensitivity |
| Random Forest       | —        | —                   | —                    | —        | Strong feature interpretation |
| XGBoost             | —        | —                   | —                    | —        | Often best overall |
| Neural Network      | —        | —                   | —                    | —        | Good complexity handling |

*(Exact values depend on your run and can be added here.)*

### 📌 Typical Findings (based on UCI Adult dataset):
- **XGBoost** or **Random Forest** usually give the **highest accuracy**.  
- Neural Networks perform well but require more compute/time.  
- Logistic Regression is simple and interpretable but underperforms.  
- SVM works well but is computationally heavier.  
- **Education**, **age**, and **marital status** are the strongest predictors.

---

## 📈 Visualizations Included

- Income class distribution  
- EDA histograms & bar charts  
- Correlation heatmap  
- ROC Curve  
- Confusion matrices (all models)  
- Feature importance (RF, XGB)  
- Training accuracy/loss curves (Neural Network)  
- Comparison bar charts for model metrics  
- Training time comparison  

---


---

## 🏁 Conclusions

- Ensemble methods (**XGBoost, Random Forest**) consistently outperform others.  
- The dataset’s class imbalance significantly affects model performance.  
- Education, age, and marital status remain the top predictors.  
- SMOTE improves sensitivity for the minority class.  
- Neural networks perform well but require careful tuning.  

---

## 👤 Author

**Devaansh Kataria**  
M.S. in Data Science — Stony Brook University  
Focus: Applied Machine Learning, Data Analytics, Deep Learning  

---


