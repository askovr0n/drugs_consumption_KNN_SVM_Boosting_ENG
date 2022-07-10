# Cocaine consumption

- The aim of the study was to create a prediction of whether a person would use cocaine in the next month
- The training set contained 1,500 observations and 21 columns. During the data analysis process, categorical variables were split, additional interactions and variable transformations were introduced, which ultimately led to an expansion of the set to 33 columns 
- Due to university requirements, the metric that was used to measure the predictive power of the model was **balanced accuracy** (the final result achieved was 75%)
- The process of building the optimal model was based on **pipelines** in which **SMOTE** (due to a strongly unbalanced target variable) standardisation of variables (**RobustScaler**) was carried out and selection of the 15 best variables due to **mutual information**
- Performance was checked on 13 different algorithms, however, as a last resort due to university requirements, hyperparameter tuning was carried out for only three: **SVM, KNN and logistic regression**
- In order to balance the results, the **VotingClassifier** algorithm was used with a **soft parameter**, so that the predictions depended on the probability of belonging to a positive class.

Sample chart from EDA     |  Cross validation scores
:-------------------------:|:-------------------------:
![](https://github.com/askovr0n/Portfolio/blob/main/images/Project_7/EDA.png)  |  ![](https://github.com/askovr0n/Portfolio/blob/main/images/Project_7/CrossVal.png)
