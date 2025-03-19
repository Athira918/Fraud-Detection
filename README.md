# Fraud-Detection
Fraudulent activities in financial transactions pose a significant risk to banking institutions and customers. As digital transactions increase, so do fraudulent activities, making fraud detection a crucial challenge. Traditional rule-based methods often fail to detect sophisticated fraud patterns, necessitating machine learning (ML) techniques for improved accuracy and efficiency.
**Data Collection and Preprocessing**
The dataset consists of various transaction details, including transaction amounts, timestamps, customer information, and transaction types. The key preprocessing steps include:
Handling missing values through imputation or removal.
Encoding categorical features (e.g., transaction type, location, and device ID) using one-hot encoding.
Normalizing numerical features to improve model performance.
Creating a new IsFraud column based on statistical thresholding (e.g., marking the top 5% highest transactions as fraudulent).
**Exploratory Data Analysis (EDA)**
EDA provides insights into fraud patterns, helping in feature selection. We:
Visualized fraud distribution using histograms and box plots.
Analyzed correlations between features using a heatmap.
Examined the imbalance in fraud vs. non-fraud transactions using count plots
**Model Selection and Training**
A supervised classification approach was adopted to train the model. The steps include:
Splitting data into training (80%) and testing (20%) sets.
Training a Random Forest Classifier, which is robust for imbalanced datasets.
Evaluating model performance using metrics such as accuracy, precision, recall, and F1-score.
Tuning hyperparameters to enhance performance.
**Results**
The model achieved high accuracy in detecting fraudulent transactions. Key findings include:
Accuracy: 98.5%
Precision: 92.3%
Recall: 85.7%
F1-Score: 88.9%
The confusion matrix revealed that the model correctly classified most transactions but had some false positives and false negatives.
Feature importance analysis showed that TransactionAmount, TransactionType, and CustomerID were the most influential factors in predicting fraud.
**Conclusion**
This project successfully implemented a machine learning-based approach to detect fraudulent bank transactions. The Random Forest Classifier performed well in identifying fraud while minimizing false positives. However, fraud detection remains a challenging task due to evolving fraud patterns.
