# 🏦 Bank Marketing Campaign Prediction using PySpark

## 📌 Overview

The **Bank Marketing Campaign Prediction** project uses distributed data processing and machine learning to analyze customer information and predict whether a customer is likely to subscribe to a **term deposit**.

The project demonstrates an end-to-end machine learning workflow using **PySpark**, including data preprocessing, feature engineering, model training, prediction, and model evaluation.

---

## 🎯 Project Objective

The main objective is to analyze banking customer data and build a classification model that can predict customer subscription behavior.

The project aims to:

* Analyze customer demographics and financial information
* Understand factors influencing term-deposit subscriptions
* Process data using PySpark
* Build and compare machine learning classification models
* Evaluate model performance using multiple classification metrics
* Identify limitations such as class imbalance
* Support data-driven marketing decisions

---

## 📊 Dataset Overview

The project uses the **Bank Marketing (`bank.csv`)** dataset.

| Column      | Description                                                |
| ----------- | ---------------------------------------------------------- |
| `age`       | Age of the customer                                        |
| `job`       | Type of job                                                |
| `marital`   | Marital status                                             |
| `education` | Education level                                            |
| `default`   | Whether the customer has credit in default                 |
| `balance`   | Average yearly account balance                             |
| `housing`   | Whether the customer has a housing loan                    |
| `loan`      | Whether the customer has a personal loan                   |
| `contact`   | Type of communication contact                              |
| `day`       | Day of the month of the last contact                       |
| `month`     | Month of the last contact                                  |
| `duration`  | Duration of the last contact in seconds                    |
| `campaign`  | Number of contacts during the current campaign             |
| `pdays`     | Number of days since the customer was previously contacted |
| `previous`  | Number of previous contacts                                |
| `poutcome`  | Outcome of the previous marketing campaign                 |
| `y`         | Whether the customer subscribed to a term deposit          |

### Target Variable

The target variable is **`y`**:

* `yes` → Customer subscribed to a term deposit
* `no` → Customer did not subscribe

---

## 🛠️ Technologies Used

* **Python**
* **Apache Spark / PySpark**
* **Pandas**
* **NumPy**
* **Spark MLlib**
* **Logistic Regression**
* **Random Forest**
* **Jupyter Notebook**

---

## 🔄 Project Workflow

```text
Bank Marketing Dataset
        ↓
Data Loading
        ↓
Data Exploration
        ↓
Data Cleaning & Preprocessing
        ↓
Categorical Feature Encoding
        ↓
Feature Vector Assembly
        ↓
Train-Test Split
        ↓
Machine Learning Models
   ┌────┴───────────┐
   ↓                ↓
Logistic        Random Forest
Regression
   ↓                ↓
Predictions      Predictions
   └────┬───────────┘
        ↓
Model Evaluation
        ↓
Model Comparison
        ↓
Final Conclusion
```

---

## 🧹 Data Preprocessing

The dataset is prepared for machine learning by:

* Checking the dataset structure and data types
* Handling categorical variables
* Converting categorical values into numerical representations
* Creating a feature vector using Spark's feature engineering tools
* Converting the target variable into a numerical label
* Splitting the dataset into training and testing sets

The dataset was divided into approximately:

* **80% Training Data**
* **20% Testing Data**

---

## 🤖 Machine Learning Models

### 1. Logistic Regression

Logistic Regression was used as a classification model to predict whether a customer would subscribe to a term deposit.

The model produces:

* Predicted class
* Probability of each class
* Classification results

### 2. Random Forest

Random Forest was used as a second classification algorithm.

It combines multiple decision trees to make predictions and was used to determine whether a tree-based model could outperform Logistic Regression.

---

## 📈 Model Evaluation

Both models were evaluated using:

* Accuracy
* Precision
* Recall
* F1 Score
* Confusion Matrix

### Model Comparison

| Model                   |   Accuracy |  Precision |     Recall |   F1 Score |
| ----------------------- | ---------: | ---------: | ---------: | ---------: |
| **Logistic Regression** | **89.52%** | **87.60%** | **89.52%** | **87.83%** |
| Random Forest           |     88.47% |     84.36% |     88.47% |     83.90% |

---

## 🏆 Model Selection

Based on the current evaluation results, **Logistic Regression performed better than Random Forest** across Accuracy, Precision, Recall, and F1 Score.

Therefore, Logistic Regression was selected as the **better-performing model among the two evaluated models**.

However, the dataset contains a significant class imbalance, with substantially more customers who did not subscribe than customers who subscribed. The confusion matrix showed that identifying the minority positive class remains challenging.

Future improvements could include:

* Class weighting
* Oversampling/undersampling
* Hyperparameter tuning
* Probability threshold tuning
* Additional model comparison
* ROC-AUC and PR-AUC evaluation

---

## 💡 Key Insights

* Machine learning can be used to predict customer subscription behavior.
* PySpark enables scalable processing and machine learning workflows.
* Logistic Regression performed better than Random Forest in the current implementation.
* Accuracy alone is not sufficient for evaluating this dataset because of class imbalance.
* Precision, Recall, F1 Score, and confusion-matrix analysis provide a more complete understanding of model performance.
* Improving minority-class detection could make the model more useful for targeted marketing campaigns.

---

## 📌 Project Conclusion

In this project, machine learning models were developed to predict whether a bank customer would subscribe to a term deposit. The data was preprocessed and divided into training and testing datasets. Two classification algorithms, Logistic Regression and Random Forest, were trained and evaluated using Accuracy, Precision, Recall, F1 Score, and actual-versus-predicted classifications.

Logistic Regression performed better than Random Forest, achieving 89.52% accuracy and an F1 score of 87.83%, compared with 88.47% accuracy and an F1 score of 83.90% for Random Forest. Therefore, Logistic Regression was selected as the better-performing model among the two.

However, the confusion matrix revealed a significant class imbalance, with both models struggling to identify customers belonging to the positive class (1). This indicates that further improvements such as class weighting, resampling, threshold tuning, and hyperparameter optimization could improve the model's ability to identify potential subscribers.

---

## 📁 Project Structure

```text
Bank-Marketing-Prediction/
│
├── Dataset/
│   └── bank.csv
│
├── Notebook/
│   └── Bank_Marketing_Prediction.ipynb
│
├── README.md
│
└── requirements.txt
```

---

## 👩‍💻 Skills Demonstrated

**Python | PySpark | SQL/Data Processing | Machine Learning | Logistic Regression | Random Forest | Data Preprocessing | Feature Engineering | Classification | Model Evaluation | EDA | Statistical Analysis**

