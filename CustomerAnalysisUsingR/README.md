# Customer Attrition Prediction in Telecom

![Telecom Image](https://elearningindustry.com/wp-content/uploads/2021/10/shutterstock_1398425123.jpg)

## Introduction

Welcome to the Machine Learning Project on Customer Attrition Prediction in the Telecom Industry! In this project, we aim to analyze the factors influencing customer cancellations and develop predictive models to identify potential attrition cases. By leveraging various classification algorithms and data analysis techniques, we delve into customer behavior patterns and provide actionable insights to reduce attrition rates.

## Dataset

The dataset used for this project is the Telecom Customer Churn dataset, which provides information about various features related to telecom customers and their service usage. The dataset includes attributes such as customer tenure, contract details, family status, service types, and more.

## Objective

The primary goal of this project is to help the telecom company identify customers who are at risk of leaving its services. By analyzing historical customer data, we aim to build accurate predictive models that assist in proactively addressing customer attrition.

## Exploratory Data Analysis (EDA)

In the EDA section, we explore the dataset and uncover meaningful insights:

- Analyzing customer tenure and identifying trends between cancellations and tenure.
- Examining the impact of family status (spouse/partner and dependents) on attrition rates.
- Investigating the correlation between contract length and customer retention.
- Analyzing the influence of monthly charges on customer cancellations.
- Studying the effect of cellular service type and number of services on attrition.
- Investigating the attrition rate among senior citizens.

## Classification Models

In this section, we develop predictive models to identify potential customer attrition:

### Model 1: Logistic Regression

- We use logistic regression to predict customer attrition.
- Feature engineering techniques, such as Yeo-Johnson transformation and normalization, are applied to the data.
- Model performance is evaluated using metrics like accuracy, sensitivity, specificity, F1 score, and ROC AUC.
- ROC curve and confusion matrix visualizations provide insights into the model's performance.

### Model 2: k-Nearest Neighbors (KNN)

- We implement k-Nearest Neighbors algorithm for customer attrition prediction.
- Hyperparameter tuning is performed using a grid of neighbors.
- The best-performing model is selected based on ROC AUC.
- The model's sensitivity, specificity, and other metrics are analyzed, and a ROC curve is plotted.

### Model 3: Random Forest

- Random Forest is employed as a predictive model for attrition.
- Hyperparameter tuning includes parameters like mtry, trees, and min_n.
- The optimal model is selected based on ROC AUC performance.
- Feature importance analysis is conducted using Variable Importance Plot (VIP).

## Summary of Results

The analysis yields the following key findings and recommendations:

1. **Customer Tenure and Contracts**: New customers are more likely to cancel the service. Longer contract periods positively impact customer retention.

2. **Family Status**: Customers with spouses/partners and dependents tend to have lower attrition rates.

3. **Monthly Charges**: Higher monthly charges correlate with increased attrition rates.

4. **Service Usage**: Customers availing more services are more likely to stay with the company.

5. **Senior Citizens**: There's a higher attrition rate among senior citizens.

### Model Performance

- Among the models, KNN performs best in terms of sensitivity and false negatives.
- KNN's sensitivity of approximately 0.76 indicates its capability to identify potential attrition cases.

## Recommendations

Based on the analysis, we recommend the following actions to mitigate customer attrition:

1. **New Customer Attraction**: Introduce attractive offers and benefits for new customers.
2. **Single Customers**: Develop plans that cater specifically to customers without spouses/partners and dependents.
3. **Contract Options**: Introduce diverse contract options to cater to different customer preferences.
4. **Monthly Charges**: Implement cost-effective plans or discounts to retain high-paying customers.
5. **Service Bundles**: Offer service bundles at discounted rates to encourage multiple service adoption.
6. **Senior Citizen Benefits**: Provide benefits and incentives to retain senior citizen customers.

By implementing these recommendations, the company can enhance customer retention and ultimately improve business profitability.

## Tech Stack

The project utilizes the following technologies and libraries:

- R Programming Language
- Tidyverse (dplyr, tidyr, ggplot2)
- tidymodels (recipes, parsnip, rsample, ranger)
- kknn
- VIP (Variable Importance Plot)

**For more detailed insights and code implementation, please refer to the project file enclosed: `<machine_learning_project_template.RMD>`**
