# ML Activity 2: Loan Approval Prediction Using Logistic Regression

## 1. About the Activity

This activity is based on Binary Classification using Logistic Regression.

The main objective is to build a Logistic Regression model that predicts whether a loan application will be approved or rejected.

## 2. Dataset Information

- **Dataset Name:** Loan Prediction Problem Dataset
- **Source:** Kaggle
- **Dataset Link:** https://www.kaggle.com/datasets/altruistdelhite04/loan-prediction-problem-dataset
- **File Used:** train.csv
- **Target Column:** Loan_Status

The dataset contains information about loan applicants, such as gender, marital status, education, income, loan amount and credit history.

The target column has two classes:

- Y – Loan Approved (1)
- N – Loan Rejected (0)

## 3. Tools and Technologies Used

- Python
- Google Colab
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn

## 4. Work Completed

The following steps were performed in this activity:

1. Loaded and explored the dataset.
2. Checked missing values and duplicate records.
3. Visualized the loan approval class distribution.
4. Handled missing values.
5. Converted categorical data into numerical form.
6. Scaled the features.
7. Divided the dataset into training and testing sets using an 80:20 stratified split.
8. Studied the sigmoid function and Logistic Regression.
9. Trained the Logistic Regression model.
10. Predicted loan approval probabilities and class labels.
11. Compared different classification thresholds (0.3, 0.5 and 0.7).
12. Evaluated the model using a confusion matrix, accuracy, precision, recall, specificity and F1-score.
13. Compared the model with a majority-class baseline.
14. Plotted the ROC curve and calculated ROC-AUC.
15. Tested the model using a new applicant example.

## 5. Key Results

After running the model, the following results were obtained:

- **Accuracy:** 0.7479674796747967
- **Precision:** 0.7368421052631579
- **Recall:** 0.9882352941176471
- **F1-Score:** 0.8442211055276382
- **ROC-AUC:** 0.8417956656346749

The model's performance was also compared at different classification thresholds to understand how the threshold affects loan approval predictions.


## 6. Conclusion

In this activity, I implemented Logistic Regression for a binary classification problem using the Loan Prediction dataset.

I learned how Logistic Regression predicts probabilities, converts them into class labels and evaluates classification performance using different metrics. I also understood how changing the classification threshold affects the predictions.

## 7. Project Files

- `Loan_Approval_Logistic_Regression.ipynb` – Completed Python notebook.

## 8. Faculty GitHub ID

Submission GitHub ID: [complexiota](https://github.com/complexiota)

## 9. Student Repository

This repository is created and maintained individually for the ML Activity 2 submission.
