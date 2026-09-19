# 📊 Bank Loan Default Prediction

### Machine Learning Classification Project

This project focuses on predicting whether a borrower is likely to **default on a loan** using machine learning classification techniques.

The project covers the complete machine learning workflow, from data preparation and exploratory analysis to feature engineering, model training, evaluation, and hyperparameter tuning.

---

## 🎯 Project Objective

The main objective is to build a machine learning model that can identify borrowers who are at higher risk of loan default.

Accurate default prediction can help financial institutions:

* Identify high-risk borrowers
* Improve credit risk assessment
* Support lending decisions
* Reduce potential financial losses
* Better understand factors associated with loan defaults

---

## 📂 Dataset

The project uses a loan default dataset containing information about borrowers and their loan characteristics.

The dataset includes variables related to areas such as:

* Loan information
* Borrower characteristics
* Income
* Credit history
* Loan amount
* Interest rate
* Employment
* Debt-related information
* Default status

The target variable represents whether the borrower **defaulted on the loan**.

---

# 🔄 Project Workflow

The project follows these main stages:

```text
Data Collection
      ↓
Data Preparation
      ↓
Exploratory Data Analysis
      ↓
Feature Engineering
      ↓
Train/Test Split
      ↓
Model Training
      ↓
Model Evaluation
      ↓
Hyperparameter Tuning
      ↓
Final Model
```

---

## 1. 🧹 Data Preparation

The first step was preparing the dataset for machine learning.

This included:

* Loading the dataset
* Inspecting the data
* Checking data types
* Identifying missing values
* Checking duplicate records
* Handling categorical variables
* Preparing numerical features
* Removing unnecessary columns
* Preparing the target variable

The cleaned dataset was then prepared for model training.

---

## 2. 🔎 Exploratory Data Analysis

Exploratory Data Analysis was performed to understand the dataset and identify patterns related to loan defaults.

The analysis included:

* Distribution of the target variable
* Numerical feature distributions
* Categorical feature analysis
* Correlation analysis
* Default patterns
* Outlier investigation
* Relationship between borrower characteristics and default

Visualizations were used to make the patterns easier to understand.

---

## 3. ⚙️ Feature Engineering

Additional features were created to improve the predictive information available to the models.

Feature engineering focused on relationships between existing variables, such as:

* Income and loan amount
* Debt-related measures
* Credit-related information
* Borrower financial characteristics

The goal was to provide the models with more meaningful information about borrower risk.

---

## 4. 🤖 Machine Learning Models

Multiple classification models were trained and compared.

The project explored models including:

### Logistic Regression

Used as a baseline classification model and provides an interpretable approach to binary classification.

### Decision Tree

A tree-based model that learns decision rules from the input features.

### Random Forest

An ensemble learning model that combines multiple decision trees to improve predictive performance and robustness.

---

## 5. 📏 Model Evaluation

The models were evaluated using classification metrics such as:

* Accuracy
* Precision
* Recall
* F1-score
* Confusion Matrix

Because loan default prediction can involve imbalanced classes, **precision and recall** were also considered instead of relying only on accuracy.

### Why these metrics matter

**Precision**

Measures how many borrowers predicted as defaulters actually defaulted.

**Recall**

Measures how many of the actual defaulters were successfully identified.

**F1-score**

Provides a balance between precision and recall.

---

## 6. 🌲 Random Forest Tuning

The Random Forest model was further improved through hyperparameter tuning.

A parameter grid was used to test different combinations of model settings.

The tuned model used:

```python
RandomForestClassifier(
    class_weight="balanced",
    random_state=42,
    n_jobs=-1
)
```

### Why `class_weight="balanced"`?

Loan default datasets can contain an imbalance between default and non-default cases.

Using:

```text
class_weight="balanced"
```

helps the model give greater consideration to the minority class instead of being heavily influenced by the majority class.

---

## 📊 Results

The final models were compared using their evaluation metrics to determine how well they identified loan defaults.

The final evaluation included:

* Classification reports
* Confusion matrices
* Model comparison
* Tuned Random Forest performance

The tuned model was selected based on the evaluation results from the project rather than relying on accuracy alone.

---

# 🛠️ Technologies Used

| Technology          | Purpose                   |
| ------------------- | ------------------------- |
| 🐍 Python           | Programming language      |
| 🐼 Pandas           | Data manipulation         |
| 🔢 NumPy            | Numerical operations      |
| 📊 Matplotlib       | Data visualization        |
| 📈 Seaborn          | Statistical visualization |
| 🤖 Scikit-learn     | Machine learning          |
| 📓 Jupyter Notebook | Development & analysis    |
| 🐙 Git & GitHub     | Version control           |

---

# 📁 Project Structure

```text
Week-4-Loan-Default/
│
├── Loan_Default.ipynb
├── Loan_default.csv
├── README.md
│
├── visuals/
│   ├── class_distribution.png
│   ├── correlation_matrix.png
│   ├── confusion_matrix.png
│   └── ...
│
└── requirements.txt
```

*File names can be adjusted to match the actual files in the repository.*

---

# 🧠 Key Learning Outcomes

Through this project, I practiced:

* Data cleaning
* Exploratory Data Analysis
* Feature engineering
* Classification
* Handling imbalanced datasets
* Model comparison
* Hyperparameter tuning
* Random Forest
* Model evaluation
* Confusion matrix analysis
* Precision and recall
* Machine learning workflow

---

# 💡 Business Application

Loan default prediction has practical applications in financial services.

A predictive system could potentially help lenders assess borrower risk before approving loans.

For example:

```text
Borrower Information
        ↓
Machine Learning Model
        ↓
Default Risk Prediction
        ↓
Risk Assessment
        ↓
Better Lending Decisions
```

Such models should be used as **decision-support tools**, with appropriate financial, legal, and fairness considerations rather than as the sole basis for lending decisions.

---

# 🚀 Future Improvements

Possible improvements include:

* More advanced feature engineering
* Cross-validation
* XGBoost or other boosting models
* Hyperparameter optimization
* ROC-AUC and PR-AUC analysis
* SHAP-based model explainability
* More detailed error analysis
* Model deployment using Streamlit
* Real-time loan risk prediction API

---

# 📌 Project Summary

This Week 4 project demonstrates a complete **machine learning classification pipeline for loan default prediction**.

Starting with raw borrower data, the project progresses through:

**Data Preparation → EDA → Feature Engineering → Classification → Evaluation → Random Forest Tuning**

The project provided practical experience in building and evaluating machine learning models for a real-world financial prediction problem.


---

