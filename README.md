# Credit Default Prediction Model

This project develops a logistic regression model to predict credit default using the German Credit Data from the UCI Machine Learning Repository. It includes data preprocessing, binary classification with scikit-learn and statsmodels, and model evaluation through AUC and ROC analysis.

## 📊 Dataset
- Source: [UCI Machine Learning Repository](https://archive.ics.uci.edu/ml/datasets/statlog+(german+credit+data))
- 1,000 observations
- 20 input variables (categorical and numerical)
- Target variable: 1 = good credit, 0 = bad credit

## ⚙️ Methods Used
- Logistic Regression (scikit-learn)
- Logistic Regression (statsmodels - Logit)
- Dummy encoding for categorical features
- Model evaluation with:
  - Confusion matrix
  - Classification report
  - ROC Curve
  - AUC Score

## 📈 Key Results
- AUC Score: **0.80** (Logistic Regression)
- Top features influencing default probability identified by the Logit model
- Logistic model shown to be more appropriate than OLS for binary classification

## 🔍 Further Improvements
- Feature selection using statistical criteria or recursive elimination
- Hyperparameter tuning with cross-validation
- Testing more advanced models: Random Forests, XGBoost, etc.

## 📁 Files Included
- `PROJETO 1.ipynb`: Jupyter notebook with full analysis
- `README.md`: Project description and structure

## 🧠 Conclusion
Logistic regression was successfully applied to predict creditworthiness. The project demonstrates the importance of choosing the correct model for binary classification problems and provides a solid foundation for future improvements using more advanced machine learning techniques.
