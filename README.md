 BINARY CLASSIFICATION USING LOGISTIC REGRESSION

## 1. Aim

To build a Logistic Regression model for a binary classification problem using the Loan Prediction dataset. The model predicts whether a loan application will be approved or rejected based on applicant details.

## 2. Dataset Description

**Dataset Name:** Loan Prediction Problem Dataset

**Source:** Kaggle – Analytics Vidhya Loan Prediction Problem

**Dataset File:** `train.csv`

**Target Variable:** `Loan_Status`

The dataset contains information about loan applicants, such as applicant income, co-applicant income, loan amount, loan amount term, credit history, and other details.

The target variable has two classes:

- 0 – Loan Rejected (N)
- 1 – Loan Approved (Y)

**Type of Dataset:** Structured tabular dataset

**Type of Problem:** Binary Classification

## 3. Data Loading and Inspection

The dataset was loaded using the Pandas library in Google Colab.

The following operations were performed:

- Displayed the first five rows of the dataset.
- Checked the number of rows and columns using `shape`.
- Checked column names and data types using `info()`.
- Checked missing values using `isnull().sum()`.

The dataset was inspected to understand its structure before applying the machine learning model.

## 4. Data Preprocessing

Data preprocessing was performed to prepare the dataset for Logistic Regression.

The following steps were carried out:

1. Checked and handled missing values.
2. Removed the unnecessary `Loan_ID` column.
3. Converted categorical values into numerical values using encoding.
4. Separated the independent variables (X) and dependent variable (y).
5. Divided the dataset into training and testing data using an 80:20 ratio.
6. Applied feature scaling where required.

The target variable `Loan_Status` was converted into numerical form:

- N = 0
- Y = 1

## 5. Logistic Regression Model

Logistic Regression is a supervised machine learning algorithm used for classification problems.

It predicts the probability that an input belongs to a particular class.

Unlike Linear Regression, which predicts continuous values, Logistic Regression predicts probabilities between 0 and 1.

The Sigmoid function is used to convert the output into a probability.

**Sigmoid Function:**

```text
σ(z) = 1 / (1 + e^(-z))
```

Where:

- z = weighted sum of input features
- e = mathematical constant
- σ(z) = predicted probability

If the predicted probability is greater than or equal to 0.5, the applicant is classified as approved. Otherwise, the applicant is classified as rejected.

## 6. Model Training and Prediction

The Logistic Regression model was created using the Scikit-learn library.

The model was trained using the training dataset and tested using the testing dataset.

After training, the model predicted the loan approval status for the test data.

The model also generated probability values for loan approval.

## 7. Model Evaluation

The model was evaluated using different classification evaluation metrics.

The following results were obtained:

| Evaluation Metric | Result |
|---|---:|
| Accuracy | 74.80% |
| Precision | 73.68% |
| Recall | 98.82% |
| F1-Score | 84.42% |
| ROC-AUC Score | 84.18% |

**Explanation of Evaluation Metrics:**

1. **Accuracy:** Measures the overall percentage of correct predictions.
2. **Precision:** Measures how many predicted positive cases were actually positive.
3. **Recall:** Measures how many actual positive cases were correctly identified.
4. **F1-Score:** Represents the balance between precision and recall.
5. **ROC-AUC:** Measures how well the model distinguishes between the two classes.

## 8. Confusion Matrix

A confusion matrix is used to compare actual class labels with predicted class labels.

It contains four values:

- True Positive (TP): Correctly predicted approved applications.
- True Negative (TN): Correctly predicted rejected applications.
- False Positive (FP): Rejected applications incorrectly predicted as approved.
- False Negative (FN): Approved applications incorrectly predicted as rejected.

**Confusion Matrix Result:**

<img width="662" height="567" alt="image" src="https://github.com/user-attachments/assets/e75dcfe6-d01d-4012-a6cc-af1f6f6db30c" />


**Specificity Formula:**

```text
Specificity = TN / (TN + FP)
```

**Specificity Result:**0.526316

## 9. Threshold Comparison

The classification threshold is used to convert predicted probabilities into class labels.

Different thresholds such as 0.3, 0.5, and 0.7 were considered to understand how changing the threshold affects classification results.

| Threshold | Accuracy | Precision | Recall | F1-Score |
|---|---|---|---|---|
| 0.3 | 0.7479674796747967 | 0.7368421052631579 | 0.9882352941176471 | 0.8442211055276382 |
| 0.5 | 0.8455284552845529 | 0.8235294117647058 | 0.9882352941176471 | 0.8983957219251337 |
| 0.7 | 0.8617886178861789 | 0.84 | 0.9882352941176471 | 0.9081081081081082 |

The final threshold should be selected based on the actual comparison results and the purpose of the classification.

## 10. ROC Curve

The ROC curve is used to evaluate the performance of a binary classification model at different classification thresholds.

It represents:

- True Positive Rate (TPR) on the Y-axis.
- False Positive Rate (FPR) on the X-axis.

The ROC-AUC score obtained by the model was **0.8418**.

This indicates that the model has a good ability to distinguish between approved and rejected loan applications.

## 11. Conclusion

In this activity, a Logistic Regression model was implemented to predict loan approval using the Loan Prediction dataset.

The dataset was inspected and preprocessed before training the model. The model predicted whether a loan application would be approved or rejected.

The performance was evaluated using accuracy, precision, recall, F1-score, confusion matrix, and ROC-AUC.

The model achieved an accuracy of approximately 74.80% and an ROC-AUC score of 0.8418.

Thus, this activity helped in understanding binary classification, Logistic Regression, probability prediction, classification thresholds, and model evaluation.

## 12. Decision Log

During the implementation of the Logistic Regression model, the following decisions were made:

| Sr. No. | Decision Taken | Reason |
|---|---|---|
| 1 | Selected the Loan Prediction dataset. | It contains applicant details and loan approval status. |
| 2 | Selected `Loan_Status` as the target variable. | It represents whether a loan is approved or rejected. |
| 3 | Converted N and Y into 0 and 1. | Logistic Regression requires numerical target values. |
| 4 | Removed unnecessary columns. | To avoid using irrelevant information during model training. |
| 5 | Divided the dataset into training and testing sets in an 80:20 ratio. | To train the model and evaluate it on unseen data. |
| 6 | Selected Logistic Regression. | It is suitable for binary classification problems. |
| 7 | Used 0.5 as the initial classification threshold. | It provides a standard starting point for converting probabilities into class labels. |
| 8 | Evaluated the model using accuracy, precision, recall, F1-score and ROC-AUC. | To understand the model's classification performance. |

## 10. GitHub Submission Information
**Submission GitHub ID:** [complexiota](https://github.com/complexiota)

**Repository Name:** `Activity1_Multiple_Linear_Regression_[YourRollNumber]`

**Repository Visibility:** Public

**Student:** Purva Pangarkar  
**Activity:** Logistic Regression
