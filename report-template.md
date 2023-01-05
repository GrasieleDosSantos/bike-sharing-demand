# Report: Predict Bike Sharing Demand with AutoGluon Solution
#### Grasiele Batista Dos Santos

## Initial Training
### What did you realize when you tried to submit your predictions? What changes were needed to the output of the predictor to submit your results?
TODO: Negative values had to be set to zero because negative demand does not make sense.

### What was the top ranked model that performed?
TODO: The top ranked model was the Weighted Ensemble one.

## Exploratory data analysis and feature creation
### What did the exploratory analysis find and how did you add additional features?
TODO: In the EDA we have realized, for example, that the demand increases during workdays. Also, temperature has an almost normal distribution. I have created two extra features from the column "datetime": hour and month. The histogram of the feature "hour" showed us that there were 3 moments during the day where the demand would have a sharp increase (considering that the hour zero is identified with the hour 24).

### How much better did your model preform after adding additional features and why do you think that is?
TODO: The root mean squared decreased from approx. 71 to 12.7 when adding the two extra features. This is because they have a high explanatory power, as we could guess from their distributions.

## Hyper parameter tuning
### How much better did your model preform after trying different hyper parameters?
TODO: we had a slight increase in the root mean squared error, that went from 12.7 to 26.3 when compared to case where we only added the extra variables. However, the kaggle score was slightly better, going from 0.64 to 0.52.

### If you were given more time with this dataset, where do you think you would spend more time?
TODO: Probably in the EDA and feature engineering.

### Create a table with the models you ran, the hyperparameters modified, and the kaggle score.
|model|hpo1|hpo2|hpo3|score|
|--|--|--|--|--|
|initial|?|?|?|?|
|add_features|?|?|?|?|
|hpo|?|?|?|?|

### Create a line plot showing the top model score for the three (or more) training runs during the project.

TODO: Replace the image below with your own.

![model_train_score.png](img/model_train_score.png)

### Create a line plot showing the top kaggle score for the three (or more) prediction submissions during the project.

TODO: Replace the image below with your own.

![model_test_score.png](img/model_test_score.png)

## Summary
TODO: We have found that the Weighted Ensemble was the model that performed best in our context, and that feature engineering was crucial in obtaining a better performance. Hyperparameter optimization did not increase the performance, even after 3 different choices of parameters.
