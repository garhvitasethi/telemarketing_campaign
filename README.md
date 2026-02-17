# Portuguese Bank Telemarketing Campaign Analysis

A machine learning project analyzing the effectiveness of a Portuguese bank's telemarketing campaigns for term deposit subscriptions. This project uses classification algorithms to predict customer conversion and identify key factors influencing campaign success.

## Project Overview

The analysis focuses on predicting whether a client will subscribe to a term deposit based on various demographic and campaign-related features.

### Business Problem
- Optimize marketing campaign effectiveness
- Identify high-potential customers for term deposits
- Reduce campaign costs by targeting the right audience
- Understand key factors driving customer decisions

## Key Findings

- **Best Model Performance**: Random Forest Classifier
  - Feature importance analysis revealed that `balance` and `age` are the top predictors
  - Achieved strong predictive performance across multiple metrics
- **Logistic Regression**: Provided baseline performance with good interpretability
- **Key Insights**: Customer account balance and age are the most significant factors in predicting term deposit subscriptions

## Technical Implementation

### Models Used
1. **Logistic Regression**
   - Solver: SAGA
   - Max iterations: 5000
   - Cross-validated with Stratified K-Fold (5 splits)

2. **Random Forest Classifier**
   - 100 estimators
   - Feature importance analysis performed
   - Full preprocessing pipeline with StandardScaler

### Evaluation Metrics
- Accuracy
- Precision
- Recall
- F1 Score
- ROC AUC Score

### Data Preprocessing
- One-hot encoding for categorical variables
- Standard scaling for numerical features
- Train-test split (80/20)
- Handled missing values with forward fill

## Repository Structure

```
marketing-campaign-analysis/
├── README.md                          # Project documentation
├── requirements.txt                   # Python dependencies
├── notebooks/
│   └── telemarketing_campaign.ipynb       # Main analysis notebook
├── reports/                           # Project reports and presentations
└── data/
    └── README.md                      # Data source information
```


### Prerequisites
- Python 3.7+
- Jupyter Notebook or Google Colab


## Dataset Information

**Source**: [UCI Machine Learning Repository - Bank Marketing Dataset](https://archive.ics.uci.edu/ml/datasets/Bank+Marketing)

**Citation**: 
Moro, S., Cortez, P., & Rita, P. (2014). A data-driven approach to predict the success of bank telemarketing. Decision Support Systems, 62, 22-31.

The dataset contains information about direct marketing campaigns (phone calls) of a Portuguese banking institution. The classification goal is to predict if the client will subscribe to a term deposit.

**Features include**:
- Demographic data (age, job, marital status, education)
- Financial information (balance, housing loan, personal loan)
- Campaign data (contact type, duration, number of contacts)
- Previous campaign outcomes

## Key Features Identified

Based on Random Forest feature importance analysis:

1. **Balance** (70.2% importance) - Customer account balance
2. **Age** (25.0% importance) - Customer age
3. **Job Categories** - Particularly blue-collar, student, and retired
4. **Marital Status** - Married and single customers showed different patterns

## Results Summary

The analysis demonstrates that:
- Financial indicators (balance) are the strongest predictors
- Demographic factors (age) play a significant secondary role
- Campaign strategy can be optimized by targeting specific customer segments
- Machine learning models can effectively predict customer conversion


This project is available for educational purposes. The dataset is publicly available from the UCI Machine Learning Repository.

[GS]
This project was completed as part of an Analytical Marketing course.

