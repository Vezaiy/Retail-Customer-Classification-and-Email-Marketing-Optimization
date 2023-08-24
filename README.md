Customer Classification for Email Marketing Opt-In Prediction
This repository presents a comprehensive analysis using classification models to predict customer outcomes in an imbalanced setting, specifically focusing on customer decisions regarding email marketing opt-in. The project delves into understanding the factors that drive customers to opt into email marketing versus opting out. The analysis takes into account a range of customer demographics, shopping behaviors, and spending patterns across various departments.

Project Objective
The main goal of this project is to uncover the underlying reasons behind customer choices regarding email marketing opt-in. By leveraging a dataset containing over 52,000 sales entries spanning multiple departments and several customer attributes (age, post code, gender, shopping frequency, and departmental spending), the project aims to answer whether customers who opt into email marketing already exhibit higher spending habits or if the opt-in decision leads to increased spending. To achieve this, a series of informative features are engineered from the data, capturing diverse aspects of customer demographics and behavior. Classification models are then employed to predict outcomes based on these features, offering insights into the key drivers influencing customers to opt in.

Data Overview
The dataset encompasses sales data from a span of two years (2019 to early 2021) and includes transaction records across multiple departments. Each customer is characterized by unique attributes such as post code, age, gender, shopping frequency, and average spending across different departments.

Project Workflow
The project follows a structured workflow, beginning with data exploration and cleaning. Key stages of the workflow are as follows:

Feature Engineering:

Creation of Customer Duration: Time interval between the first and last transactions.
One-Hot Encoding: Transformation of post code data, customer gender, and department sales frequencies into binary indicators.
Standardization of Variables: Standardization applied to specific variables, such as post code and age, while preserving sparsity.
Class Imbalance Handling:

The initial dataset exhibited a significant class imbalance between customers opting into email marketing (majority class) and those opting out (minority class).
To address this issue, the minority class was oversampled with replacement to achieve a balanced representation.
An alternative approach involving downsampling the majority class was also tested but yielded inferior results.
Model Selection and Comparison:

A range of classification models were selected for initial evaluation:
Naive Bayes (baseline)
Logistic Regression
Decision Tree Classifier
Random Forest Classifier
K-nearest Neighbors
Support Vector Classifier
XGBoost Classifier
Soft & Hard Voting Classifiers
Model performance was assessed through cross-validation (5 folds) on the training data, primarily using accuracy as the evaluation metric.
Model Tuning and Selection:

The Support Vector Classifier emerged as the top performer with an accuracy of 90% on the training data and approximately 96% on the test data.
Hyperparameter tuning was conducted to optimize the model's performance further.
Conclusion
This project provides valuable insights into customer behavior related to email marketing opt-in decisions. By employing advanced classification techniques, the analysis sheds light on the factors driving customers to opt in or out of email marketing. The final tuned Support Vector Classifier achieved an impressive accuracy level, underscoring its effectiveness in predicting customer outcomes in this context.
- Support Vector Classifier
- XGBoost Classifier
- Soft & Hard Voting Classifiers

#### the final result is the tuned support vector classifier as the clear winner with 90% accuracy on the training data and ~96% on the test data
