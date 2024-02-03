# **Optimizing Grocery Retail: A Time Series Forecasting Approach for Favorita Stores Sales**
#### Time series forecasting is an effective technique for predicting future values using previous data that has a time component. Precise sales forecasting can be the difference between success and stagnation in the dynamic retail industry. Imagine being able to accurately plan promotions, optimize inventory, and predict client demand.
## **Business Understanding**
#### This project centers on delving into historical sales data, constructing and evaluating machine learning models to uncover patterns, and identify factors influencing store sales. By tackling key business questions related to seasonality, promotions, store locations, and economic factors, the aim is to deliver actionable recommendations for inventory management, marketing strategies, and overall business optimization. The project's journey involves building and evaluating various machine learning models, with the ultimate goal of selecting the most effective model to make accurate predictions for future sales.
### Analytical Questions
1. What is the sales distribution across different store clusters?
2. What product families contribute the most to the overall sales across all stores?
3. What was the impact of the earthquake on the sales?
4. What is the correlation between promotion frequency and total sales for each store?
5. What is the sales trend by year, month, week and day?
6. What is the overall sales trend?
   
#### We will take the following methodical approach in order to meet the goals:
## **Data Exploration**:
#### To comprehend the available features, their distributions, and their interactions, thoroughly examine the datasets that have been provided. In addition to helping find any problems with the data quality, this stage will offer preliminary insights into the store sales statistics.

## **Data Preparation**:
#### Encode categorical variables as needed, handle missing values, and carry out feature engineering. Techniques including scaling, one-hot encoding, and imputation may be used in this step.

## **Model Selection and Training**:
#### Using the given data, choose suitable time series forecasting models and train them. To improve forecasting accuracy, think about adding outside variables like sales, holidays, and oil prices, if any are available.

## **Model Evaluation**:
#### Apply suitable metrics, such as root mean square log error(RMSLE), mean absolute error (MAE), root mean square error (RMSE), or mean absolute percentage error (MAPE), to assess the trained models. Determine which forecasting model is the most accurate and dependable by evaluating the models' performance.

## **Model Deployment and Forecasting**:
#### Using the test dataset that has been supplied, deploy the selected model to forecast shop sales for upcoming intervals. Provide estimates for the intended time frame and evaluate the model's accuracy in capturing sales trends.

## **Files used and their description**
#### train.csv: contains time series data, such as store_nbr, family, onpromotion, and the target variable sales.
#### test.csv: The test data has the same features as the training data. The task is to predict the target sales for the dates in this file.
#### transaction.csv: This file includes the date, store_nbr, and the number of transactions made on each specific date.
#### oil.csv: contains daily oil prices which is very important because Ecuador is an oil-dependent country, and its economy is imparted greatly by oil price flactuatuions.
#### holidays_events.csv: This file provides information about holidays and events.
#### stores.csv: This file contains store data, including city, state, type, and cluster.
#### Additionally, an earthquake with a magnitude of 7.8 struck Ecuador on April 16, 2016. The earthquake led to relief efforts and donations, which significantly impacted supermarket sales for several weeks afterwards.

## **Data Preparation**
#### *Managing missing values: Locate the missing values in the datasets and choose a suitable handling plan for them. This could entail deleting data points that have missing values or imputing missing values.
#### *Feature engineering is the process of transforming and creating additional variables that may enhance the models' ability to forecast the future. This stage could involve producing interaction terms, scaling numerical variables, or encoding categorical variables.

## Model Training and Development
#### Utilizing the prepared data, some models are trained and, if available, include outside variables. By adjusting the hyperparameters and choosing the top-performing model, the best model is selected for prediction with the test dataset.

## Model Evaluation
#### The trained models are evaluated using appropriate metrics such as RMSLE, MAE, RMSE, MSE, or MAPE. Interpret the models to understand the factors driving store sales and their relative importance.
## **SUMMARY**
#### Predicting sales for different stores using past data is the aim of this time-series forecasting research. The dataset contains data on family classifications, store specifics, promotions, and economic variables like oil prices. An examination of exploratory data provided insights into the sales distribution, pointing out possible seasonality and temporal fluctuations. The analysis included using machine learning models, displaying sales patterns, and finding connections using Python and well-known tools like Pandas, Plotly, and Scikit-Learn. Since the Root Mean Squared Logarithmic Error (RMSLE) is appropriate for distributions with skews, it was selected as the evaluation metric. The time series was made stationary by using a variety of methods, including as scaling and differencing. Of all the models that were trained, Random Forest Regressor proved to be the best perforing model with a RMSLE of 0.22 after tuning. This model was saved for future predictions on the test dataset, ensuring proper preprocessing using saved encoders and scalers. The project aims to provide accurate sales forecasts for effective business planning.









