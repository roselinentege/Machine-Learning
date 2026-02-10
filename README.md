Machine Learning in Finance: Predictive Modeling & Optimization
WorldQuant University | MSCFE 632 | Group 12406

Project Objective
This project addresses the core challenges of building robust financial models: preventing models from "cramming" (overfitting) and ensuring they can navigate market "noise" to find actionable signals. We specifically explored hyperparameter optimization, the bias-variance tradeoff, and ensemble methods to improve predictive accuracy.

Issues Addressed
1. Hyperparameter Optimization
Challenge: Preventing models from becoming "trapped" by noise.
Solution: Implemented Grid Search CV in Python to find the perfect method.
Optimization: Tuned Support Vector Machine (SVM) parameters to balance model simplicity with accuracy.

2. Bias-Variance Tradeoff

Concept: High bias leads to underfitting (too simple), while high variance leads to overfitting (distracted by noise).
Goal: Finding the "middle ground" where a model generalizes well to future market data.

3. Ensemble Methods

Approach: Combined multiple models (Bagging, Boosting, and Stacking) to make predictions safer by trusting a "team" rather than one voice.
Key Tools: Evaluated AdaBoost and XGBoost as part of a relay-race style chain where each model corrects the previous one's errors.

Performance Results
We compared three primary models to determine the most effective predictor:
The Top Performer: The Support Vector Machine (SVM) was the most successful model, achieving a high accuracy of 0.8950.
Alternative Models: Logistic Regression followed with an accuracy of 0.8000, while the AdaBoost Ensemble achieved 0.7400.
Model Reliability: With an overall F1-score of 0.89, the SVM demonstrated it was correct many times and is highly reliable for this financial dataset.

SVM Performance
Precision (Accuracy of Predictions): The model achieved a precision of 0.91 for non-default cases (Class 0) and 0.88 for default cases (Class 1).
Recall (Ability to Find All Cases): The model successfully identified 90% of actual non-defaults and 89% of actual defaults.
Confusion Matrix Breakdown: Out of the test samples, the model correctly predicted 102 non-defaults and 77 defaults, with only a small number of errors (11 and 10 respectively).

Why These Results Matter for Investors
Balanced Prediction: The high precision and recall scores show the model isn't just "guessing" the most common outcome; it is actually learning the difference between the two classes.
Market Alpha: By focusing on "signal" over "noise," this model provides better risk control and higher trust for investors making live decisions.
