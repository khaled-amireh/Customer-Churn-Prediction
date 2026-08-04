# Customer Churn Prediction using Logistic Regression

Machine Learning classification project that predicts whether a customer is likely to churn based on customer behavior and subscription information.

---

## Overview

Customer churn prediction helps businesses identify customers who are likely to leave a service. In this project, I built a complete machine learning pipeline using Logistic Regression, starting from data preprocessing and ending with model evaluation.

---

## Dataset

The dataset contains customer information such as:

- Age
- Gender
- Subscription Type
- Contract Length
- Tenure
- Usage Frequency
- Support Calls
- Payment Delay
- Total Spend
- Last Interaction

Target Variable:

- **Churn**
  - 0 → Customer stays
  - 1 → Customer leaves

---

## Project Workflow

### 1. Import Libraries

Imported the required Python libraries for:

- Data manipulation
- Data visualization
- Data preprocessing
- Model training
- Model evaluation

Libraries used:

- NumPy
- Pandas
- Matplotlib
- Scikit-learn

---

### 2. Load the Dataset

Loaded the dataset using Pandas and separated the features from the target variable.

Also removed the **CustomerID** column because it is only an identifier and does not provide useful information for prediction.

---

### 3. Exploratory Data Analysis (EDA)

Performed a quick exploration of the dataset by checking:

- Dataset information
- Data types
- Statistical summary
- Missing values

This step helps understand the data before preprocessing.

---

### 4. Split the Dataset

The dataset was split into:

- 80% Training Set
- 20% Testing Set

The split was done before preprocessing to prevent data leakage.

---

### 5. Data Preprocessing

#### One-Hot Encoding

Categorical features were transformed using **OneHotEncoder**.

Encoded columns:

- Gender
- Subscription Type
- Contract Length

One-Hot Encoding converts categorical values into numerical binary features that can be used by machine learning algorithms.

---

### 6. Feature Scaling

Applied **StandardScaler** on the numerical features.

Feature scaling was performed because Logistic Regression is a distance-based optimization algorithm and performs better when numerical features are on a similar scale.

---

### 7. Train the Model

Trained a **Logistic Regression** classifier using the training dataset.

---

### 8. Make Predictions

Predicted customer churn on the testing dataset.

---

### 9. Model Evaluation

Evaluated the model using:

- Confusion Matrix
- Accuracy Score
- Classification Report

Final Accuracy:

**83.16%**

---

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Scikit-learn
- Jupyter Notebook

---

## Project Structure

```
Customer_Churn_Prediction/
│
├── customer_churn_prediction.ipynb
├── customer_churn_dataset-testing-master.csv
├── README.md
```

---

## Results

The Logistic Regression model achieved an accuracy of **83.16%** on the test set.

Evaluation metrics included:

- Accuracy
- Precision
- Recall
- F1-Score
- Confusion Matrix

These metrics provide a better understanding of the model's performance than relying on accuracy alone.

---

## Future Improvements

Possible improvements for this project include:

- Trying different classification algorithms
- Hyperparameter tuning
- Feature selection
- Cross-validation
- ROC Curve and AUC Score
- Precision-Recall Curve
