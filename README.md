# Credit Card Fraud Detection Model

## Overview
This repository contains a machine learning model for predicting credit card fraud. The model utilizes transaction data, including transaction time, transaction features (V1-V26), transaction amount, and transaction class (0 for legitimate transactions, 1 for fraudulent transactions), to classify transactions as either legitimate or fraudulent. The model was trained using logistic regression and achieved an accuracy score of 91%.

## Dataset
The dataset used for training and testing the model contains transaction information, with each row representing a single transaction. The features include:
- Time of transaction
- Transaction features V1-V26 (anonymized)
- Transaction amount
- Transaction class (0 for legitimate transactions, 1 for fraudulent transactions)

## Steps Taken
1. **Dependencies**: Imported necessary libraries such as numpy, pandas, sklearn, and joblib for model training and evaluation.
2. **Data Cleaning**: Ensured that the dataset did not contain any missing values by checking with `df.isnull().sum()`.
3. **Class Balancing**: Addressed class imbalance by sampling the class with significant data and concatenating it with the other class with lesser data.
4. **Data Splitting**: Split the dataset into features (X) and labels (Y) for training and testing the model.
5. **Model Training**: Utilized logistic regression for modeling the credit card fraud detection.
6. **Model Evaluation**: Achieved an accuracy score of 91%, indicating high model performance.

## Files Included
- `credit_card_fraud_detection.ipynb`: Jupyter Notebook containing the code for data preprocessing, model training, and evaluation.
- `credit_card_fraud_detection.py`: Python script equivalent of the Jupyter Notebook for easy execution.
- `credit_card_fraud_detection.pkl`: Serialized model file saved using joblib for future use.
- `archive (1).zip`: Sample dataset containing credit card transaction information.

## Usage
To use the model for credit card fraud detection:
1. Clone the repository to your local machine.
2. Install the required dependencies using `pip install -r requirements.txt`.
3. Run the `credit_card_fraud_detection.py` script or open the `credit_card_fraud_detection.ipynb` notebook in a Jupyter environment.
4. Provide transaction data to the model for prediction.
5. The model will output predictions indicating whether the transaction is legitimate or fraudulent.

## Conclusion
This machine learning model provides a reliable solution for detecting credit card fraud by accurately classifying transactions as legitimate or fraudulent. Further enhancements and optimizations can be made to improve the model's performance and scalability.

For any questions or feedback, feel free to contact the repository owner.
