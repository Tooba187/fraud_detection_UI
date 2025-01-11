# fraud_detection_UI

Fraud Detection System
Overview
This project aims to develop a fraud detection system that identifies fraudulent transactions using machine learning techniques. The system is trained on a dataset such as the Credit Card Fraud Dataset, which includes features like transaction amount, time, and other variables that can be used to classify a transaction as legitimate or fraudulent.

The project leverages a Random Forest or Gradient Boosting model to detect fraudulent transactions. The system's performance is evaluated using precision, recall, and F1-score metrics, and a simple command-line interface is provided for testing the model with new data.

Dataset
The project uses the Credit Card Fraud Dataset, which contains transaction data with features such as:

Time: Time elapsed between the first transaction and the current transaction.
Amount: The monetary value of the transaction.
Class: The target variable indicating whether the transaction is fraudulent (1) or legitimate (0).
The dataset is highly imbalanced, with fraudulent transactions accounting for only a small percentage of all transactions.

Steps
1. Data Preprocessing
Handling Imbalanced Data: Due to the nature of the dataset, where fraudulent transactions are much fewer, techniques like SMOTE (Synthetic Minority Over-sampling Technique) or undersampling are applied to balance the classes.
Feature Scaling: The Amount and Time features are standardized to bring them to the same scale, ensuring the model can learn efficiently.
2. Model Training
Random Forest: This model is trained using the processed data. Random Forest, an ensemble method, is used due to its ability to handle complex relationships and imbalanced datasets effectively.
Gradient Boosting: As an alternative, Gradient Boosting models like XGBoost can be used for their accuracy and performance in classification tasks.
3. Model Evaluation
The performance of the model is evaluated using the following metrics:

Precision: The proportion of correctly predicted fraudulent transactions to all predicted fraudulent transactions.
Recall: The proportion of correctly predicted fraudulent transactions to all actual fraudulent transactions.
F1-score: The harmonic mean of precision and recall, providing a single metric to evaluate model performance.
4. Testing Interface
A simple command-line interface (CLI) allows users to test the fraud detection system. The user inputs the transaction amount and time, and the system predicts whether the transaction is fraudulent or not. The interface also provides feedback based on the model’s prediction.

5. Output
The final output of the system includes:

Model Evaluation Metrics: Precision, recall, and F1-score metrics for assessing model performance.
Transaction Prediction: A prediction on whether a given transaction is fraudulent or legitimate.

Results
The trained model's performance can be measured by:

Precision: High precision indicates that the model is good at identifying fraudulent transactions without misclassifying legitimate transactions.
Recall: A high recall value indicates that the model is effective at catching most fraudulent transactions.
F1-score: This combines precision and recall, providing an overall metric for the model's performance.
