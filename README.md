# Report: Predict Bike Sharing Demand with AutoGluon Solution
#### KAMDEM CHOUDJEM IDRISS

## Initial Training
### What did you realize when you tried to submit your predictions? What changes were needed to the output of the predictor to submit your results?
When I tried to submit my predictions for my result I noticed that my public and private score improved
furthermore and I changed the default value of hyper parameters and hyperparameter_tune_kwargs
in the fit() function

### What was the top ranked model that performed?
The top ranked modelthat performed is "LightGBMLarge_BAG_L2" according to my last submission

## Exploratory data analysis and feature creation
### What did the exploratory analysis find and how did you add additional features?
The exploratory analysis showed a certain seasonality in the data and a Gaussian distribution of values associated with categorical features such as: atemp, temp, humidity, windspeed.
during descriptive and data exploration I was able to highlight very distinct categories with the "value_count()" function, then this allowed me to add new features

### How much better did your model preform after adding additional features and why do you think that is?
The model has significantly improved for the better by showing great performance in its score which was submitted on the leaderboard and this happened because I created new features which highlight the detail of seasonality and which highlights the subcategories of the data having a Gaussian distribution

## Hyper parameter tuning
### How much better did your model preform after trying different hyper parameters?
the model improved even more after hyper parameters tuning of the model which were changed

### If you were given more time with this dataset, where do you think you would spend more time?
I will spend more time to researching the best hyperparameter pairs to refine the performance of the model even further.

### Create a table with the models you ran, the hyperparameters modified, and the kaggle score.
| model            | hpo1 |   hpo2    |   hpo3  | score  |
|------------------|------|-----------|---------|--------|
| initial          | 600  | default   | default | 1.84751|
| add_features     | 800  | default   | default | 0.64893|
| hpo              | 1000 | multimodal| bayesopt| 0.49393|

### Create a line plot showing the top model score for the three (or more) training runs during the project.

TODO: Replace the image below with your own.

![model_train_score.png](/model_training_score.png)

### Create a line plot showing the top kaggle score for the three (or more) prediction submissions during the project.

TODO: Replace the image below with your own.

![model_test_score.png](/model_test_score.png)

## Summary
Exploratory data analysis is a better way to better understand the data and thus apply feature engineering which will subsequently allow our model to find the pattern that best describes its data.
moreover, the fine-tuning of the hyper parameters allows our model to refine its modeling precision on the entire dataset.
