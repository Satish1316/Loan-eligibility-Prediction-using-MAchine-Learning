

# Loan Eligibility Prediction Using Machine Learning

This project focuses on building a predictive model that determines whether a loan applicant is eligible for a loan based on certain features. The prediction is based on various factors such as income, loan amount, credit history, and other applicant-related information. This project was built in a Jupyter Notebook using Python and various machine learning libraries.

## 1. Overview
The **Loan Eligibility Prediction** project aims to assist financial institutions in assessing the risk associated with lending to potential borrowers. By analyzing historical data and using machine learning algorithms, the project predicts whether an applicant is likely to be approved for a loan or not.

The project uses the **Naive Bayes** classification algorithm to build the predictive model, along with exploratory data analysis (EDA) to better understand the data and features that influence loan eligibility.

## 2. Project Goals
- Analyze the dataset to understand key patterns and insights.
- Develop a machine learning model to predict loan eligibility.
- Evaluate the model's performance using various metrics such as accuracy, precision, and recall.
- Provide recommendations for improving the loan approval process based on the model's predictions.

## 3. Dataset Overview
The dataset used in this project contains the following columns related to applicant and loan information:

- **ApplicantIncome**: Income of the loan applicant.
- **CoapplicantIncome**: Income of the co-applicant (if any).
- **LoanAmount**: Loan amount requested by the applicant.
- **Loan_Amount_Term**: Duration of the loan in months.
- **Credit_History**: Whether the applicant has a good credit history (1 for good, 0 for bad).
- **Gender**: Gender of the applicant (Male/Female).
- **Married**: Marital status of the applicant.
- **Dependents**: Number of dependents the applicant has.
- **Education**: Education level of the applicant (Graduate/Non-Graduate).
- **Self_Employed**: Whether the applicant is self-employed or not.
- **Property_Area**: Type of area where the property is located (Urban/Semiurban/Rural).
- **Loan_Status**: Target variable, whether the loan was approved or not (Y/N).

## 4. Data Preprocessing
Data preprocessing is a crucial step before building the model. The following tasks were performed:
- Handling missing values by imputing with appropriate strategies (mean/median/mode).
- Encoding categorical variables such as **Gender**, **Marital Status**, **Property Area**, etc., using **Label Encoding** and **One-Hot Encoding**.
- Feature scaling of numerical columns such as **Loan Amount** and **Applicant Income** to ensure uniformity in the data.
- Splitting the dataset into training and testing sets for model evaluation.

## 5. Model Building
### Algorithm Used:
- **Naive Bayes Classifier**: A probabilistic machine learning algorithm that was chosen for its simplicity and efficiency with categorical features.
  
The model was trained on the training dataset, and the following steps were performed:
1. **Fitting the Model**: The Naive Bayes model was trained using the preprocessed training data.
2. **Prediction**: The model was used to predict loan eligibility for the test dataset.
3. **Evaluation**: Model performance was evaluated using metrics like **accuracy**, **precision**, **recall**, and **F1-score**.

## 6. Model Evaluation
The performance of the model was evaluated using the following metrics:
- **Accuracy**: The percentage of correctly predicted loan statuses.
- **Confusion Matrix**: Provides insight into the number of true positives, true negatives, false positives, and false negatives.
- **Precision and Recall**: Used to measure the relevance of predictions and the ability to identify eligible loan applicants.
- **F1-Score**: Harmonic mean of precision and recall, providing a balanced measure of the model's performance.

### Results:
- **Accuracy**: 85% on the test dataset.
- **Precision**: 0.82 (for loan-approved cases).
- **Recall**: 0.87 (for loan-approved cases).
- **F1-Score**: 0.84.

## 7. Insights from the Project
- **Credit History** is one of the most significant factors in determining loan eligibility.
- **Applicant Income** and **Loan Amount** have a moderate correlation with loan approval, suggesting higher incomes tend to get loans approved more frequently.
- **Self-employed applicants** are less likely to be approved compared to salaried applicants, likely due to income stability concerns.
- The **Naive Bayes classifier** performed well in classifying loan eligibility, achieving a high level of accuracy with minimal tuning.

## 8. Project Outcomes
- Developed a machine learning model capable of predicting loan eligibility with a high level of accuracy.
- Provided key insights that could help financial institutions in improving their loan approval processes.
- Demonstrated the importance of credit history and income stability in determining loan approval outcomes.
  
## 9. Future Improvements
- Implement other machine learning algorithms (e.g., Random Forest, Decision Trees) to compare performance with the Naive Bayes classifier.
- Use a larger and more diverse dataset for better generalization of the model.
- Explore advanced feature engineering techniques to improve the model’s accuracy further.

