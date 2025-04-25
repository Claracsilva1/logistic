# 🧾 Credit Default Prediction Model

A logistic regression model was developed to predict credit default using the German Credit Data from the UCI Machine Learning Repository. This project applies both `scikit-learn` and `statsmodels` to perform binary classification and evaluate model performance through key statistical metrics.

---

## 📊 Dataset Overview

- **Source**: [UCI Machine Learning Repository](https://archive.ics.uci.edu/ml/datasets/statlog+(german+credit+data))
- **Observations**: 1,000
- **Features**: 20 variables (categorical and numerical)
- **Target**:  
  - `1`: Good credit  
  - `0`: Bad credit (converted from original class `2`)

---

## ⚙️ Methodology

- Data preprocessing with dummy variable encoding  
- Train/test split using `train_test_split()`  
- Logistic regression using:
  - `LogisticRegression` (from `scikit-learn`)
  - `Logit` model (from `statsmodels`)  
- Model evaluation using:
  - Confusion matrix  
  - Classification report (precision, recall, F1-score)  
  - ROC curve and AUC score  
  - Coefficient significance (p-values from Logit)

---

## 📈 Key Results

- **AUC Score**: ~0.80 (Logistic Regression)  
- **Statistically significant predictors** identified via the Logit model  
- Logistic regression confirmed to be more appropriate than OLS for binary classification due to probability constraint (0 ≤ 𝑃 ≤ 1)

---

## 🧠 Insights & Conclusion

The logistic regression model demonstrated strong predictive performance, achieving an AUC score of approximately **0.80**.

Key insights derived from the statistical analysis include:

- **Account status (`account_status_A14`)** was the most influential variable in predicting credit risk. Clients without a checking account had a significantly higher likelihood of defaulting.
- **Credit amount (`credit_amount`)** showed a strong positive association with default probability. Applicants requesting larger loans were more likely to default.
- **Loan duration (`duration`)** was also positively correlated with default. Longer-term loans tended to carry higher risk.
- **Employment duration** and **personal status** had marginal statistical relevance in this dataset and may require further exploration or external validation.

These results illustrate the value of logistic regression not only as a predictive tool, but also as a means to interpret which factors most significantly impact financial behavior. This type of analysis can inform credit risk policies and support data-driven decision-making in financial institutions.

Overall, the project reinforces that **selecting the appropriate model for binary classification** (i.e., logistic regression instead of OLS) is essential for producing interpretable and operationally valuable results in credit risk analysis.

---

## 🔧 Potential Future Enhancements

- Feature selection based on correlation analysis or recursive elimination  
- Cross-validation and hyperparameter tuning  
- Implementation of more complex models:
  - Random Forest  
  - Gradient Boosting (XGBoost, LightGBM)

---

## 📂 Files Included

- `PROJETO 1.ipynb` – Full Jupyter notebook with preprocessing, modeling and evaluation  
- `README.md` – Project documentation and summary

---


