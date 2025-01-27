# Score Prediction for T-20 cricket matches using regression
The building of score predictor model wherein past performance data of the teams have been taken into consideration along with the existing state of match. Post feature selection and hyperparameter tuning linear regression was implemented along with ensemble learning family algorithms - Random Forest and XGBoost. Our XGBoost model has surpassed the performance of other two algorithms with a MAE score of 1.67 and RMSE as 3.52. 

## Stages:
- Extraction: extracted data from kaggle cricsheet in yaml format 
- Transformation: feature extraction
- Predcition: Regression models for best predictiom
  
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

## Regression Model Evaluation

In this project, I compared the performance of various regression models on a dataset. Below are the evaluation metrics for each model:

| **Algorithm**           | **Validation** | **Tuning** | **MAE**  | **MSE**  | **RMSE** |
|-------------------------|----------------|------------|----------|----------|----------|
| **Linear Regression**    | Yes            | No         | 13.07    | 314.8    | 17.74    |
| **RF Regression**        | Yes            | Yes        | 2.44     | 24.27    | 4.92     |
| **XGBoost Regression**   | Yes            | Yes        | 1.67     | 12.45    | 3.52     |

### Key Takeaways:

- **XGBoost Regression** outperformed both Linear Regression and Random Forest, achieving the lowest MAE, MSE, and RMSE. This was expected given the dataset's non-linear patterns.
- **Random Forest Regression** performed well but was not as accurate as XGBoost, likely due to XGBoost’s ability to capture more complex interactions.
- **Linear Regression** was the baseline model and showed significantly higher error rates, suggesting that a simple linear model was insufficient for this problem.

### Model Tuning:
- Hyperparameter tuning was performed for both Random Forest and XGBoost using **Grid Search** to find the best configuration, leading to the improved results.

## Credits:
- The code guidance for this project (https://github.com/campusx-official/cricket-score-predictor/tree/main)



