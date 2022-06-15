# HDB Flats Price Analysis and Prediction using Machine Learning

What factors affect HDB resale prices?

The dataset and problem statement were taken from this Kaggle competition: https://www.kaggle.com/competitions/hdbresale

## Data Pre-processing
Response variable: resale_price

<img width="612" alt="image" src="https://user-images.githubusercontent.com/19891445/173773243-3b66b7f1-b5e8-4349-98e9-34e83fb00dc1.png">

## Prediction Methodology
The Models we have tried were Linear Regression, LASSO regression, Ridge Regression, DecisionTree, Random Forest, XGBoost. We evaluated these models by mainly RMSE (root mean squared error). At first, we just went through each model without hyperparameter tuning and compared the prediction results. After selecting the one that provided best result, we conducted hyperparameter tuning methods (GridSearchCV,　RandomizedSearchCV) to improve the accuracy of our prediction.

<img width="609" alt="image" src="https://user-images.githubusercontent.com/19891445/173773512-2bdef806-5939-48df-8b45-b1874e72baef.png">

## Results
By comparing the results of each model as shown in the Table below, we could get the best performance from XGBoost. As the loss curve shown in the figure, we can not observe overfitting after hyperparameter tuning. Thus, we are able to expect an appropriate prediction result from this prediction model.

<img width="647" alt="image" src="https://user-images.githubusercontent.com/19891445/173773559-245ba002-4038-4fe0-aa44-a5964d9b12bd.png">

Final Kaggle accuracy score:  0.97248
