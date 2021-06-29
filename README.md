# Machine Learning - Exoplanet Exploration


## Background

This project is to study the NASA Kepler space telescope data based on a planet-hunting mission. I created several machine learning models that are capable of classifying candidate exoplanets from the raw dataset.

### Preprocess the Data

* Preprocess the dataset before fitting the model.
    - unnecessary columns have removed
    - all rows containing NaN are removed
    - Data is 25/75 split into a training and test set.
    - Numerical data is scaled accordingly (MinMaxScaler)
* Perform feature selection and remove unnecessary features.
    - Uses tree and randomforest to sort the features based on feature_importance, but none of the features were removed for model fitting.

### Tune Model Parameters

* Use `GridSearch` to tune three classification model parameters.
    - Uses GridSearch to find the best parameters for all three models
    - The tuned model is used to make the final exoplanet prediction
    - All models score greater than 85% accuracy on test data, except for KNN model

### Results

* SVM model: Best Score = 0.8886 (Tuned)
* Random Forest model: Best Score = 0.8940 (Tuned)
* KNN model(k=19): Best Score = 0.8226 (Tuned)
* Deep Learning model: Loss = 0.2539 / Accuracy = 0.8993


- - -

© 2021 Trilogy Education Services, LLC, a 2U, Inc. brand. Confidential and Proprietary. All Rights Reserved.
