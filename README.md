# customer-churn-logistic-regression
Telecom Customer Churn Prediction using Logistic Regression
📌 Project Overview

This project predicts customer churn for a telecom company using Logistic Regression.
Customer churn refers to customers leaving a service, and predicting it helps companies take proactive actions to retain users.

The dataset contains customer demographics, account details, and service usage. The goal is to build a reliable machine learning model that predicts whether a customer will churn or not.

📂 Dataset

The project combines three datasets:

Customer Data – demographics and account info

Churn Data – churn labels and billing info

Internet Data – internet usage and service features

Total Records: 7043 customers
Churn Rate: ~27%

🔑 Steps Performed

Data Import & Merging – combined customer, churn, and internet datasets.

Data Cleaning – handled missing values, converted categorical variables to numeric, one-hot encoding.

Feature Engineering – scaled numerical features, removed multicollinearity using correlation and VIF.

Model Building – trained Logistic Regression using statsmodels and scikit-learn.

Feature Selection – applied Recursive Feature Elimination (RFE).

Model Evaluation – evaluated with accuracy, sensitivity, specificity, precision, recall, ROC-AUC.

Optimal Cutoff – determined the best probability threshold (~0.3) for balanced performance.

📊 Results

Training Accuracy: ~81%

Test Accuracy: ~78%

Sensitivity (Recall): ~63%

Specificity: ~84%

Precision: ~65%

ROC-AUC: ~0.84

The model performs well in distinguishing between churn and non-churn customers with a balanced tradeoff between recall and precision.

⚙️ Tech Stack

Python

Pandas, NumPy – data preprocessing

Matplotlib, Seaborn – visualization

Scikit-learn – model building, RFE, evaluation metrics

Statsmodels – regression summary and statistical analysis

🚀 How to Run

Clone the repository

git clone https://github.com/your-username/telecom-churn-prediction.git
cd telecom-churn-prediction


Install dependencies

pip install -r requirements.txt


Run the notebook or script to train and evaluate the model.

📌 Future Improvements

Try other models (Random Forest, XGBoost, Neural Networks)

Perform hyperparameter tuning

Use SMOTE or other techniques to handle class imbalance

Deploy the model as a web app (Flask/Streamlit)
