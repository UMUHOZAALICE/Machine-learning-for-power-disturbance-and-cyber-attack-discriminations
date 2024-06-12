# Machine Learning for Power Disturbance and Cyber Attack Discrimination

## Project Overview
The goal of this project is to classify system power disturbances into categories such as No Events, Attacks, and Natural disturbances using machine learning models. Three different models were trained for this purpose: Random Forest, Logistic Regression, and k-Nearest Neighbors (k-NN). The performance of these models was evaluated, and the benchmark model was identified.

## Dataset
The full dataset consists of 15 different datasets, each sampled at one percent (1%). The combined dataset includes 129 columns (128 features and 1 dependent variable). The features include 29 measurements from each of the 4 Phasor Measurement Units (PMUs), totaling 116 PMU measurement columns, and 12 columns for control panel logs.

## Data Analysis
- **Outliers**: The dataset contained approximately 8114 outliers, which were handled using the Interquartile Range (IQR) method.
- **Categorical Data**: Categorical data were encoded using label encoding.

## Modeling
This is a classification problem, and three models were used:
1. Random Forest
2. Logistic Regression
3. k-Nearest Neighbors (k-NN)

**K-fold Cross-Validation** was used to evaluate model performance, with 10 folds being used. Feature selection was also performed to enhance model efficiency by selecting the best features.

## Model Performance Evaluation
Different performance metrics were used to evaluate the models, including:
- Accuracy
- Precision (weighted)
- Recall (weighted)
- F1 Score (weighted)

The F1 Score was used to derive the final conclusion. The Random Forest model emerged as the benchmark model with a 64% F1 Score.

## Hyperparameter Tuning
The Random Forest model was further fine-tuned using GridSearchCV. The best parameters identified were:
- max_depth: 3
- max_leaf_nodes: 7
- n_estimators: 10

With these parameters, the model achieved an F1 Score of 61%.

## Conclusion
The Random Forest model is the best model for predicting and classifying cyber-attacks in power systems. Intelligent Electronic Devices (IEDs) like R1 through R4, which control relays and breakers, were found to be among the best features, providing relevant information from the original datasets.

Overall, the selected benchmark model is expected to improve the accuracy and performance of Industrial Control Systems (ICS) in detecting various types of cyber-attacks.
