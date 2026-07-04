# 📊 Customer Satisfaction (CSAT) Prediction Using Machine Learning

## 📌 Project Overview

Customer satisfaction is one of the most important indicators of service quality. Businesses rely on Customer Satisfaction (CSAT) scores to evaluate customer experience and identify areas for improvement.

This project develops an **end-to-end Machine Learning solution** to predict **Customer Satisfaction (CSAT) Scores (1–5)** using customer support interaction data. The model enables organizations to proactively identify customer interactions that are likely to receive lower satisfaction scores, allowing support teams to take corrective actions before customer dissatisfaction impacts business outcomes.

The project covers the complete Machine Learning workflow, including:

* Data Cleaning
* Exploratory Data Analysis (EDA)
* Feature Engineering
* Hypothesis Testing
* Feature Selection
* Data Preprocessing
* Handling Imbalanced Data
* Machine Learning Model Development
* Hyperparameter Tuning
* Model Explainability using SHAP

---

# 🎯 Business Problem

Customer support organizations usually receive customer satisfaction ratings after support interactions have ended.

This delay makes it difficult to proactively improve customer experience.

The objective of this project is to build a predictive model capable of estimating customer satisfaction immediately after a customer interaction based on operational and service-related features.

The predicted CSAT score can help businesses:

* Identify dissatisfied customers early
* Improve customer support quality
* Optimize agent performance
* Reduce customer churn
* Support data-driven business decisions

---

# 📂 Dataset Information

The dataset contains approximately **86,000 customer support interactions**.

Each record represents one customer support case.

### Target Variable

* **CSAT Score**

  * 1 = Very Dissatisfied
  * 2 = Dissatisfied
  * 3 = Neutral
  * 4 = Satisfied
  * 5 = Highly Satisfied

### Important Features

* Channel Name
* Category
* Sub-category
* Product Category
* Customer Remarks
* Item Price
* Response Time
* Handling Time
* Agent Name
* Supervisor
* Manager
* Tenure Bucket
* Agent Shift

---

# 🛠️ Project Workflow

```
Dataset
   │
   ▼
Data Cleaning
   │
   ▼
Exploratory Data Analysis
   │
   ▼
Missing Value Handling
   │
   ▼
Feature Engineering
   │
   ▼
Encoding
   │
   ▼
Feature Scaling
   │
   ▼
Train-Test Split
   │
   ▼
SMOTE
   │
   ▼
Machine Learning Models
   │
   ▼
Model Evaluation
   │
   ▼
Cross Validation
   │
   ▼
Hyperparameter Tuning
   │
   ▼
SHAP Explainability
```

---

# 📈 Exploratory Data Analysis

The following analyses were performed:

* Customer Satisfaction Distribution
* Support Channel Analysis
* Issue Category Analysis
* Product Category Analysis
* Customer City Analysis
* Agent Shift Analysis
* Tenure Bucket Analysis
* Response Time Analysis
* Item Price Analysis
* Correlation Heatmap
* Multivariate Analysis

### Key Insights

* Most customer interactions occurred through the **Inbound** support channel.
* **Returns** and **Order Related** issues were the most common customer queries.
* Most customers provided a **CSAT Score of 5**.
* The dataset showed significant class imbalance.
* Response time and operational factors strongly influenced customer satisfaction.

---

# 🧹 Data Preprocessing

The following preprocessing steps were applied:

* Duplicate Removal
* Missing Value Imputation
* Feature Engineering
* Label Encoding
* One-Hot Encoding
* Feature Scaling
* Feature Selection
* Train-Test Split (80:20)
* SMOTE for Class Balancing

---

# 📊 Hypothesis Testing

Three statistical tests were performed:

### Chi-Square Test

* Support Channel vs CSAT Score
* Issue Category vs CSAT Score

### ANOVA Test

* Item Price vs CSAT Score

These tests confirmed statistically significant relationships between customer satisfaction and several operational variables.

---

# 🤖 Machine Learning Models

Three classification models were implemented and compared.

| Model               | Purpose                |
| ------------------- | ---------------------- |
| Logistic Regression | Baseline Model         |
| Random Forest       | Ensemble Learning      |
| XGBoost             | Final Prediction Model |

---

# 📈 Model Performance

| Model               | Accuracy     |
| ------------------- | ------------ |
| Logistic Regression | 44.59%       |
| Random Forest       | 62.00%       |
| XGBoost             | **67.31%** ⭐ |

---

# 🔍 Model Evaluation Metrics

The models were evaluated using:

* Accuracy
* Precision
* Recall
* F1 Score
* Confusion Matrix
* Classification Report

---

# 🔄 Cross Validation

The final XGBoost model was evaluated using **5-Fold Cross Validation**.

**Average Accuracy**

```
69.54%
```

This demonstrates that the model generalizes well across different subsets of the dataset.

---

# ⚙️ Hyperparameter Tuning

Hyperparameter tuning was performed using **GridSearchCV**.

Optimized Parameters:

* Number of Trees
* Maximum Tree Depth
* Learning Rate

The tuned model achieved the best overall performance.

---

# 📉 Model Explainability

To improve model transparency, **SHAP (SHapley Additive Explanations)** was used.

Generated Explainability Visualizations:

* SHAP Summary Plot
* SHAP Feature Importance Plot
* SHAP Waterfall Plot

Top influential features included:

* Response Time
* Agent Shift
* Order Related Category
* Agent Name
* Tenure Bucket

---

# 💼 Business Impact

The developed model enables organizations to:

* Predict customer satisfaction immediately after customer interactions.
* Identify dissatisfied customers early.
* Improve customer support quality.
* Optimize agent performance.
* Reduce customer complaints.
* Support data-driven decision making.

---

# 🚀 Future Scope

Future improvements may include:

* Natural Language Processing (NLP) on Customer Remarks.
* Deep Learning Models.
* Streamlit Web Application.
* Azure Machine Learning Deployment.
* Real-time Prediction API.
* Continuous Model Retraining.

---

# 🖥️ Technologies Used

### Programming Language

* Python

### Libraries

* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scikit-learn
* XGBoost
* SHAP
* Imbalanced-learn

### Development Environment

* Jupyter Notebook
* Google Colab

### Version Control

* Git
* GitHub

---

# 📁 Repository Structure

```
Customer-Satisfaction-Prediction/
│
├── Dataset
│
├── Customer_Satisfaction_Prediction.ipynb
│
├── README.md
│
├── requirements.txt
```

---

# ▶️ How to Run

### Clone Repository

```bash
git clone https://github.com/yourusername/Customer-Satisfaction-Prediction.git
```

### Install Dependencies

```bash
pip install -r requirements.txt
```

### Launch Notebook

```bash
jupyter notebook
```

Open the notebook and run all cells sequentially.

---

# 📌 Results

* Successfully developed an end-to-end Machine Learning pipeline.
* Compared multiple classification algorithms.
* Selected XGBoost as the best-performing model.
* Achieved **67.31% Accuracy** after hyperparameter tuning.
* Improved model interpretability using SHAP Explainability.

---

# 👨‍💻 Author

**Abhishek Sinha**

---

## ⭐ If you found this project helpful, consider giving this repository a Star.
