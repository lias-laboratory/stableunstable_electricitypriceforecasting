# Regression Algorithms

In this section, we will test and
then discuss the regression approach-based models, specif-
ically the Multi Linear Regression model, Support Vector
Regression model, Random Forest, and XGBRegressor model.
Due to our dataset being already very good (zero outliers, zero
NaN values) the preprocessing only consist in applying the
MinMaxScaler method to normalize our data.
For the regression approach, we will use the entire dataset to
which we also added features and they consist of
- “holiday”: binary – from external data that represents if
a day was a holiday or not.
- “weekday”: binary – represents if a day was a weekday
or a weekend.
- “month”: represents the month.

We used the GridSearchCV technique to loop through
predefined hyper-parameters to test every combination and
get the best one.
We tested the models first with all the features then applied
the sequential forward selection (SFS) technique to select
attributes and test again.
Three metrics are adopted for the evaluation to later compare
the models, Mean Absolute Error (MAE), Root Mean
Absolute Error (RMSE), Coefficient of Variance (CV), and
the last metric used is the computational time.