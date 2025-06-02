<details>
<summary><strong>🔍 Methodology</strong></summary>

<br>

The following methodology outlines the structured approach used to build a predictive analytics solution for identifying patients at high risk of hospital readmission within 30 days post-discharge.

### 1. 🏗️ Problem Framing
- Defined the business objective: **Reduce avoidable readmissions** to improve patient outcomes and minimize operational costs.
- Translated the clinical question into a supervised machine learning task: **Binary classification** (readmitted vs. not readmitted).

### 2. 🧩 Data Collection & Integration
- Consolidated data from multiple sources:
  - **Electronic Health Records (EHR)**
  - **Admission & discharge logs**
  - **Patient demographics and comorbidity indicators**
- Ensured data privacy and compliance by anonymizing sensitive information.

### 3. 🧹 Data Cleaning & Preprocessing
- Handled missing values via mean/mode imputation and domain-informed defaults.
- Detected and treated outliers using IQR and z-score methods.
- Encoded categorical variables using one-hot and label encoding.
- Normalized numerical features for model stability.
- Created derived fields like:
  - Length of stay
  - Discharge hour buckets
  - Count of prior admissions

### 4. 📊 Exploratory Data Analysis (EDA)
- Analyzed key patterns across patient demographics, diagnoses, length of stay, and readmission rates.
- Visualized relationships using **Seaborn** and **Matplotlib**:
  - Correlation heatmaps
  - Age and diagnosis-based readmission rates
  - Discharge timing trends

### 5. 🧠 Feature Engineering
- Developed predictive features informed by domain knowledge:
  - Charlson Comorbidity Index
  - Time since last admission
  - Medication burden score
- Reduced multicollinearity through correlation analysis and **Variance Inflation Factor (VIF)**.

### 6. 🤖 Model Development
- Collaborated with data science team to train and evaluate several classifiers:
  - **Logistic Regression** for interpretability
  - **Random Forest** and **XGBoost** for performance
- Handled class imbalance using **SMOTE** and class weighting techniques.
- Evaluated model performance using:
  - ROC-AUC
  - F1 Score
  - Precision-Recall Curve

### 7. 🧾 Model Explainability
- Applied **SHAP** to:
  - Interpret individual predictions
  - Identify top contributing risk factors
  - Build stakeholder trust in model recommendations

### 8. 📈 Reporting & Visualization
- Designed dashboards using **Power BI** and **Tableau**:
  - Patient-level risk scores
  - Department-wise readmission trends
  - Top drivers of risk

### 9. 🔁 Feedback & Iteration
- Incorporated clinical feedback into feature design and dashboard layout.
- Monitored for model drift and retrained periodically.
- Delivered actionable insights to care teams for real-time intervention.

</details>
