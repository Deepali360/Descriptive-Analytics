# Score Prediction for T-20 cricket matches using regression
The building of score predictor model wherein past performance data of the teams have been taken into consideration along with the existing state of match. Post feature selection and hyperparameter tuning linear regression was implemented along with ensemble learning family algorithms - Random Forest and XGBoost. Our XGBoost model has surpassed the performance of other two algorithms with a MAE score of 1.67 and RMSE as 3.52.
## Functions, Library and methods used:
- Splitting the data:	sklearn .model_selection | train_test_split	| Splitting the data into training and test datasets
- Evaluation:	sklearn.metrics |	MAE, MSE, RMSE | 	To find best algorithm.
- Validation:	sklearn.model_selection	| learning_curve |T o depict training and validation score.
- Hyperparameter tuning:	sklearn.model_selection |	GridSearchCV | To find best parameters.
- Algorithms:	sklearn.linear_model | sklearn.ensemble | xgboost	
- LinearRegression | RandomForestRegressor | XGBRegressor	
- *Note:  These different algorithm used to train the data and further evaluated on the bases of MSE.*
- Standard Scaler:	sklearn.preprocessing |	Standard Scaler	| To scale the dataset
- Mathematical Operations: 	NumPy	| To find mean values 
- Graphs :	matplotlib.pyplot	| To depict learning curve, error range graphs.
- Data frame operations: 	Pandas |To manipulate data


