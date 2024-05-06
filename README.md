# Brain-Cancer
Predicts the overall survival in month for Glioma patients.

Nulls:
Dropped columns that were filled with a majority of null values and then used KNN Imputer to resolve missing values in the dataset using K-Nearest Neighbours.

Outliers:
Outliers were capped based on the IQR for the independent variables

Categorical Data --> Numerical Data: 
Transformed Catgorical data into number values using one hot encoding. 

Modeling:
Used correlation to filter the features for a linear regression model.
PCA + Linear Regression
Pipeline = RF + CV and Grid Search CV: 72
Mutual Information + Random Forest: 57.3
Mutual Information + Random Forest + Grid SearchCV: 73.8
Extreme Gradient Boost: 68%
Extreme Gradient Boost + Mutual Info Regression: 67.5
Extreme Gradient Boost + Mutual Info Regression + Grid SearchCV: 74.5
