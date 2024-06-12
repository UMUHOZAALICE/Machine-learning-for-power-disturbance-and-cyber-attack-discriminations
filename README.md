# Machine-learning-for-power-disturbance-and-cyber-attack-discriminations
This project aims to classify system power disturbances such as NoEvents, Attack and or Natural disturbances using machine learning models. Random forest, logistic regression, and k-Nearest neighbor were trained. And by evaluating Models performance, the benchmark model was exposed.

# Dataset
The full dataset for power system disturbances is made from 15 different datasets which are randomly sampled at one percent (1 %) from each dataset. The datasets consist of 129 columns (128 features, 1 dependent variable). It means 29 measurements from each phasor measurement units (PMU) which measure electrical waves on electricity grid and there are 4 PMUs which result in 116 PMU measurement columns in total and 12 columns for control panel logs.

# Data analysis
The dataset was prepared and processed whereby the datset were containing outliers around 8114 and the categorical data. The outlier were handled using Interquartile Range (IQR) while categorical data weere encoded using label encoder.

# Modeling
The task is classification problem, different classification model were used, including Random forest, Logidtic regression and K nearest neighbor. K fold cross validation technique were used to evaluate the performance of the model. K fold cross validation involves dividing the dataset into k subsets or folds of approximately equal size. In our case, 10 folds were used.

# Models Performance Evaluation 
To evaluate the model performance different perfomrance metrics were used sincluding accuracy, precision_weighted, recall_weighted, f1_weighted. To derive the conckusion, F1 socre was used. The benchmark model came to be Random forest with high score compared to others with 64% score. 

# Hyperparameter tuning
After recealing the benchmark model, it was fine tuned to the best parameters combination using GridSearchCV and the nest paramenters for the model comes to be
# Conclusion

 
