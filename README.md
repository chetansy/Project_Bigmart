# Big Mart Sales Prediction
## Business Objectives:-- 
### Sales Prediction for Big Mart Outlets
- The Data scientists at BigMart have collected 2013 sales data for 1559 products across 10 stores in different cities. Also, certain attributes of each product and store have been defined. The aim is to build a predictive model and predict the sales of each product at a particular outlet.

## Data Set Details:-- 
We have train (8523) and test (5681) data set, train data set has both input and output variable(s). You need to predict the sales for test data set.

- Train file:- CSV containing the item outlet information with sales value
- Test file: CSV containing item outlet combinations for which sales need to be forecasted

## Acceptance Criteria:--
They have the actual sales for the test dataset, against which your predictions will be evaluated. We will use the Root Mean Square Error value to judge your response.

## Strategy:--
- [Define Goal](https://github.com/chetansy/Project_Bigmart/blob/master/README.md#define-goals)
- [Explore & Visualize data](https://github.com/chetansy/Project_Bigmart/blob/master/README.md#explore--visualize-data)
- [Pre-Processing Data](https://github.com/chetansy/Project_Bigmart/blob/master/README.md#pre-processing-data)
- [Partitioning Data](https://github.com/chetansy/Project_Bigmart/blob/master/README.md#partitioning-data)
- [Apply Prediction Models](https://github.com/chetansy/Project_Bigmart/blob/master/README.md#apply-prediction-models)
- [Evaluate & Compare Models](https://github.com/chetansy/Project_Bigmart/blob/master/README.md#evaluate--compare-models)
- [Model Selection](https://github.com/chetansy/Project_Bigmart/blob/master/README.md#model-selection)

### Define Goals:-
- By using Predictive model and predict the sales of each product at a particular outlet.
- Using this model, BigMart will try to understand the properties of products and outlets which play a key role in increasing sales.

### Explore & Visualize data:- 

### Pre-Processing Data:-
- Train Data Set has 3873 Missing Values.
- Test Data Set has 2582 Missing Values
- After applying Random Forest to the entire data set, To replace values of NA.
- As we dont have a column Item_Outlet_Sales, so we will create it First with NA Value.
- We have Combined the Data with "rbind",

### Partitioning Data:-
- We have Splitted Data Into Train & Test.

### Apply Prediction Models:-
- We Have Used 3 Regression Model
1- Linear Regression Model
2- Random Forest Ranger Regression Model
3- XGBoost Regression Model

### Evaluate & Compare Models:-
- Prediction model performance will be evaluated on the basis of your prediction of the sales for the test data (test.csv), which contains similar data-points as train except for the sales to be predicted.
- We will use the Root Mean Square Error value to judge your response.

### Model Selection
We will prefer XGBoost for Predicting Model as RMSE seems to be low compared to other.
