# Loan Prediction Model

This project aims to predict whether a loan applicant is at risk of defaulting on a loan based on several features using machine learning models.

## Features

- **Id**: Unique identifier for each applicant.
- **Income**: Annual income of the applicant.
- **Age**: Age of the applicant.
- **Experience**: Number of years of professional experience.
- **Married/Single**: Marital status of the applicant (married or single).
- **House_Ownership**: Housing status of the applicant (e.g., rented, owned, or no rent/no own).
- **Car_Ownership**: Whether the applicant owns a car (yes or no).
- **Profession**: The profession of the applicant (e.g., Software Developer, Mechanical Engineer, etc.).
- **CITY**: The city where the applicant resides.
- **STATE**: The state where the applicant resides.
- **CURRENT_JOB_YRS**: Number of years in the current job.
- **CURRENT_HOUSE_YRS**: Number of years in the current residence.
- **Risk_Flag**: Binary flag indicating whether the applicant is at risk of defaulting on the loan (1 = high risk, 0 = low risk).

## Libraries Used

- `pandas`: For data manipulation and analysis.
- `sklearn`: For building and evaluating machine learning models.
  - `LogisticRegression`: For logistic regression model.
  - `RandomForestClassifier`: For random forest classifier model.
  - `train_test_split`: For splitting data into training and testing sets.
  - `LabelEncoder`: For encoding categorical features.
  - `StandardScaler`: For scaling features.
  - `accuracy_score`, `classification_report`, `confusion_matrix`: For model evaluation.
  - `cross_val_score`: For cross-validation.

## Data Preprocessing

- **Label Encoding**: Used `LabelEncoder` for encoding categorical features:
  - `Married/Single`
  - `Car_Ownership`
- **One-Hot Encoding**: Applied for other categorical variables.
- **Feature Scaling**: Scaled features using `StandardScaler` to ensure they have a mean of 0 and standard deviation of 1.

## Models Used

### Logistic Regression
- Accuracy: 57.73%
  
### Random Forest Classifier
- Accuracy: 90.14%

## Evaluation Metrics

- **Accuracy Score**: Measures the percentage of correctly classified instances.
- **Classification Report**: Provides precision, recall, and F1-score for each class.
- **Confusion Matrix**: A matrix showing the true positive, false positive, true negative, and false negative values.

