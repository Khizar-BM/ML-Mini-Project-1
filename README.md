# Bank Marketing Campaign Prediction

## Project Overview

This project analyzes a Portuguese banking institution's direct marketing campaigns (phone calls) to predict whether a client will subscribe to a term deposit. The aim is to build and evaluate different machine learning models that can effectively predict the outcome of marketing calls.

## Dataset

The dataset used is "Bank Marketing" from the UCI Machine Learning Repository, which includes client data, campaign information, and economic attributes:

- **Client attributes**: age, job type, marital status, education, etc.
- **Campaign information**: contact type, month, day, duration, etc.
- **Social and economic context attributes**: employment variation rate, consumer price index, etc.
- **Target variable**: 'y' (whether the client subscribed to a term deposit)

## Machine Learning Models

Three models were implemented and compared:
1. **Logistic Regression**
2. **Random Forest**
3. **XGBoost**

The models were evaluated using various metrics including:
- Precision
- Recall
- F1-Score
- Accuracy
- ROC-AUC

## Key Findings

- The dataset is imbalanced with only ~11% positive responses
- Top features that influence the outcome include:
  - Age
  - Interest rates (euribor3m)
  - Campaign communication frequency
  - Employment indicators
- SMOTE was used to address class imbalance
- Feature selection improved model performance
- Economic indicators significantly impact campaign success

## Repository Contents

- `ML_Mini_Project_1_Solved.ipynb`: Jupyter notebook with all code, analysis, and visualizations
- `ML Mini Project 1 Report.pdf`: Detailed report on the project, methodology, and findings
- `bank-additional-full.csv`: The dataset used for analysis
- `README.md`: This file

## Project Workflow

1. **Data Loading and Exploration**
   - Loading data
   - Initial exploration and visualization
   - Statistical summary

2. **Data Preprocessing**
   - Handling categorical variables
   - Feature scaling
   - Feature selection
   - Addressing class imbalance

3. **Model Implementation**
   - Training multiple models
   - Hyperparameter tuning
   - Model validation

4. **Evaluation**
   - Performance metrics comparison
   - Feature importance analysis
   - Model interpretation

5. **Conclusion**
   - Key insights
   - Recommendations for marketing strategy

## Requirements

The project requires the following Python libraries:
- pandas
- numpy
- scikit-learn
- matplotlib
- seaborn
- xgboost
- imbalanced-learn (for SMOTE)

## Author

Muhammad Khizar Bin Muzaffar

## License

This project is available for academic and research purposes.
