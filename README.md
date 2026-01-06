# customer-churn-prediction
Machine learning project to predict telecom customer churn using feature engineering and model tuning
# Customer Churn Prediction

This project predicts customer churn in the telecom domain using machine learning techniques.

## Objectives
- Identify customers likely to churn
- Apply feature engineering based on domain knowledge
- Compare baseline and tuned models
- Optimize recall for churn customers

## Techniques Used
- Exploratory Data Analysis (EDA)
- Feature Engineering
- One-Hot Encoding
- Logistic Regression
- Random Forest (tuned for recall)

## Key Insights
- Customers with shorter tenure are more likely to churn
- Month-to-month contracts show higher churn
- High monthly charges increase churn risk

## Tools
- Python
- Pandas, NumPy
- Scikit-learn
- Matplotlib, Seaborn

## Model Tuning & Business Considerations

Since the dataset is imbalanced, accuracy alone is not sufficient for evaluating churn prediction.
Missing a churn customer is more costly than incorrectly flagging a non-churn customer.

To address this, the Random Forest model was tuned using class weighting and tree depth constraints
to prioritize recall for churn customers. This improved the model’s ability to identify customers
at risk of churning, even at the cost of a slight reduction in overall accuracy.

Model selection was based on business impact rather than metric optimization alone.

## Future Work
- Add neural network model
- Experiment with threshold tuning
