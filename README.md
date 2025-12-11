# Predicting Annual Medical Insurance Costs

This project aims to utilize characteristic lifestyle data such as BMI and smoking history to predict an individual’s health insurance cost using machine learning models. This will provide insight into which attributes have the strongest effect on healthcare expenses, help improve cost forecasting for insurance providers, and highlight how lifestyle choices impact medical costs.

---

## Authors
- **Christian Bammann** – Contributor of data preprocessing, LR/SVM model development, and co-author of the written final project report.  
- **Ryan Monroe** – Contributor of data preprocessing, ANN model development, and co-author of the written final project report.

---

## Contents

| File                                                                                     | Description                                                 |
|------------------------------------------------------------------------------------------|-------------------------------------------------------------|
| `Predicting_Annual_Medical_Insurance_Costs_LR_SVM.ipynb`                                 | Python notebook with LR and SVM Models                      |
| `Predicting_Annual_Medical_Insurance_Costs_ANN.ipynb`                                    | Python notebook with ANN Model                              |
| `Predicting_Annual_Medical_Insurance_Costs.pdf`                                          | IEEE-style technical report                                 |
| `Predicting_Annual_Medical_Insurance_Costs_Presentation.pdf`                             | Presentation                                                |
| `insurance.csv`                                                                          | Added Dataset                                               |
| `README.md`                                                                              | Project Summary                                             |
  
---

## Results

| Model                               | Mean Squared Error (MSE)    | Mean Absolute Error (MAE)   | R² Score                    | 
|-------------------------------------|-----------------------------|-----------------------------|-----------------------------|
| Linear Regression (LR)              | 0.176                       | 0.263                       | 0.790                       |
| Support Vector Machine (SVM)        | 0.107                       | 0.156                       | 0.872                       |
| Artificial Neural Network (ANN)     | 0.125                       | 0.194                       | 0.861                       |

---

## Analysis

- The Linear Regression (LR) model performed the worst. LR struggles with nonlinear data relationships.
- The Support Vector Machine (SVM) model performed well. SVM models excel on small nonlinear datasets.
- The Artificial Neural Network (ANN) model performed the best. ANN requires a larger amount of data and more tuning.

## Key Insights

- Individuals who smoked had significantly higher charges than those who do not smoke
- Age is the second strongest factor, with older individuals tending to have higher charges
- Higher BMI often corresponds to higher charges, especially when greater than 30
- Children, sex, and region have relatively minor influence on charges compared to the features above

---

## Conclusion
These machine learning models provide evidence of contributing factors to higher medical bills and insight on what medical costs to expect based on your lifestyle. The trained models could effectively be used to predict the annual medical charges someone can expect to incur, given only their smoker status, BMI, and age. For nonsmokers who are not obese the predictions will be exceptionally accurate, and the results can be used to reinforce lifestyle habits and promote active saving for expected expenses.
