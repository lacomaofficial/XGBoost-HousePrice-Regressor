# House Price Prediction with XGBoost

This repository contains a machine learning model built with XGBoost to predict house prices using Melbourne housing data. The model is trained on various features such as 'Distance', 'Bedroom2', 'Postcode', 'Landsize', 'BuildingArea', 'YearBuilt', 'Lattitude', 'Longtitude', 'Bathroom', 'Car', and 'Propertycount'.

## Dataset

The dataset, `melb_data.csv`, contains information about different houses in Melbourne, including their attributes and sale prices.

## Data Preprocessing

The initial step involves imputing missing values in the 'Car', 'BuildingArea', and 'YearBuilt' columns using an iterative imputer.

## Model Training and Evaluation

A random forest regressor is trained on the preprocessed data to estimate house prices. The feature importance analysis reveals that the 'Distance' and 'Bedroom2' features have the highest impact on price prediction.

A more advanced XGBoost model is then trained and evaluated using the root mean squared error (MSE) and R-squared (R2) metrics. The model performs well with an R2 score of approximately 0.81 on the validation set.

## Hyperparameter Optimization

A grid search is performed to find the best hyperparameters for the XGBoost model. The best combination is found to be 'learning_rate': 0.1, 'max_depth': 5, and 'n_estimators': 300. The optimized model achieves a slightly improved R2 score of approximately 0.82 on the validation set.

## Cross-Validation

The model's performance is further evaluated using cross-validation with five folds. The average MSE is approximately 96.25 billion, and the R2 score is around 0.92, indicating the model's generalization capability.

Feel free to explore! 

![pexels-julia-foroni-4664660](https://github.com/lacomaofficial/XGBoost-HousePrice-Regressor/assets/132283879/32330c0f-ff39-4d87-970e-41a007ac4ca7)
