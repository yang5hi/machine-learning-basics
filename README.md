# Machine Learning - Exoplanet Exploration


### Before You Begin


4. Save your best model to a file. This will be the model used to test your accuracy and used for grading.

5. Commit your Jupyter notebooks and model file and push them to GitHub.


## Background

Over a period of nine years in deep space, the NASA Kepler space telescope has been out on a planet-hunting mission to discover hidden planets outside of our solar system.

To help process this data, you will create machine learning models capable of classifying candidate exoplanets from the raw dataset.

In this homework assignment, you will need to:

1. [Preprocess the raw data](#Preprocessing)
2. [Tune the models](#Tune-Model-Parameters)
3. [Compare two or more models](#Evaluate-Model-Performance)

- - -

## Instructions

### Preprocess the Data

* Preprocess the dataset prior to fitting the model.
    - unnecessary columns are removed
    - all rows containing NaN are removed
    - Data is correctly split into a training and test set
    - Numerical data is scaled accordingly (MinMaxScaler)
* Perform feature selection and remove unnecessary features.
    - Unses some form of feature selection method to identify insignificant variables (feature_importance, RFE, backwards elemination, etc.)
    - Remove insignificant variables and retrain models with the significant features
* Use `MinMaxScaler` to scale the numerical data.
* Separate the data into training and testing data.

### Tune Model Parameters

* Use `GridSearch` to tune model parameters.
    - Uses GridSearch or some hyperparameter tuning to find the best parameters for the model
    - The tuned model is used to make the final exoplanet prediction
    - Model scores greater than 85% accuracy on test data
* Tune and compare at least two different classifiers.
    - Creates, trains, and tests 3 different classification models
    - Correctly sets x and y (koi_disposition) variables
    -

### Reporting

* Create a README that reports a comparison of each model's performance as well as a summary about your findings and any assumptions you can make based on your model (is your model good enough to predict new exoplanets? Why or why not? What would make your model be better at predicting new exoplanets?).
    - README compares each of the models' performances and predictions
    - README summarizes the findings and makes suumptions based on the data and their models.
    - README descusses the predictions of the possible exoplanets with their models.

- - -

## Resources

* [Exoplanet Data Source](https://www.kaggle.com/nasa/kepler-exoplanet-search-results)

* [Scikit-Learn Tutorial Part 1](https://www.youtube.com/watch?v=4PXAztQtoTg)

* [Scikit-Learn Tutorial Part 2](https://www.youtube.com/watch?v=gK43gtGh49o&t=5858s)

* [Grid Search](https://scikit-learn.org/stable/modules/grid_search.html)

- - -

## Hints and Considerations

* Start by cleaning the data, removing unnecessary columns, and scaling the data.

* Not all variables are significant be sure to remove any insignificant variables.

* Make sure your `sklearn` package is up to date.

* Try a simple model first, and then tune the model using `GridSearch`.

* When hyper-parameter tuning, some models have parameters that depend on each other, and certain combinations will not create a valid model. Be sure to read through any warning messages and check the documentation

- - -

## Submission

* Create a Jupyter Notebook for each model and host the notebooks on GitHub.

* Create a file for your best model and push to GitHub

* Include a README.md file that summarizes your assumptions and findings.

* Submit the link to your GitHub project to Bootcamp Spot.

* Ensure your repository has regular commits (i.e. 20+ commits) and a thorough README.md file

## Rubric

[Unit 21 Rubric - Machine Learning Homework - Exoplanet Exploration](https://docs.google.com/document/d/1IcLYc8KHt82ftMcsueM6s7rn9nexuN4PqHSJDUa7e2Y/edit?usp=sharing)

- - -

© 2021 Trilogy Education Services, LLC, a 2U, Inc. brand. Confidential and Proprietary. All Rights Reserved.
