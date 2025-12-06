# Predicting-Annual-Medical-Insurance-Costs

This project aims to utilize characteristic lifestyle data such as BMI and smoking history to predict an individual’s health insurance cost using machine learning models. This will provide insight into which attributes have the strongest effect on healthcare expenses, help improve cost forecasting for insurance providers, and highlight how lifestyle choices impact medical costs.

---

## Authors
- **Christian Bammann** – Contributor of data preprocessing, Linear Regression/SVM model development, and co-author of the written final project report.  
- **Ryan Monroe** – Contributor of data preprocessing, ANN model development, and co-author of the written final project report.

---

## Contents

| File                                                                                     | Description                                                 |
|------------------------------------------------------------------------------------------|-------------------------------------------------------------|
| `Predicting_Annual_Medical_Insurance_Costs.ipynb`                                        | Main Python notebook                                        |
| `Predicting_Annual_Medical_Insurance_Costs.pdf`                                          | IEEE-style technical report                                 |
| `Predicting_Annual_Medical_Insurance_Costs_Presentation.pdf`                             | Presentation Slides                                         |
| `insurance.csv`                                                                          | Dataset                                                     |
| `README.md`                                                                              | Project Summary                                             |
  
---

## Results

| Model                               | MSE    | MAE    | R²     | 
|-------------------------------------|--------|--------|--------|
| Linear Regression                   | 0.176 | 0.263 | 0.790 |
| Support Vector Machine              | 0.107 | 0.156 | 0.872 |
| Artificial Neural Network           | 0.160 | 0.257 | 0.822 |

---

## Analysis

- The Linear Regression (LR) model performed the worst. LR struggles with nonlinear data relationships.
- The Support Vector Machine (SVM) model performed the best. SVM models excel on small nonlinear datasets.
- The Artificial Neural Network (ANN) model performed well. ANN requires a larger amount of data and more tuning.

## Key Insights

- Individuals who smoked had significantly higher charges than those who do not smoke
- Age is the second strongest factor, with older individuals tending to have higher charges
- Higher BMI often corresponds to higher charges, especially when greater than 30
- Children, sex, and region have relatively minor influence on charges compared to the features above

---

## Conclusion
The quickest and easiest way to identify apparent trends in a dataset is to apply a simple linear regression model. However, the results are nothing more than can be predicted intuitively. There is an inherent subjectiveness in the dataset that makes accurate predictions difficult.

Therefore, to thoroughly analyze underlying patterns it becomes necessary to utilize a neural network. Structuring a neural network comes with its own challenges, such as ensuring it’s complex enough to learn features yet still resistant to overfitting and exploding gradients. 

Our models provide evidence of contributing factors to higher medical bills and insight on what medical costs to expect based on your lifestyle.


