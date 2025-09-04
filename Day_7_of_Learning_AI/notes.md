Welcome to my day 7/100  of Learning AI
Today I am exploring the topics that were left tomorrow about the data preprocessing.

### 1. OrdinalEncodor
OrdinalEncoder converts ordered categorical features (like Low < Medium < High) into integers that preserve the order:
Low -> 0
Medium -> 1
High -> 2
This is different from OneHotEncoder (which makes separate 0/1 columns and does not imply order). Use Ordinal only when the categories truly have an order.
If the data don't have the natural order,then don't use the ordinalencodor,instead use the onehotencodor

### 2.RobustScaler
Its just like the standardScaler but its best when the data has more outliers.
Unlike the Standardscaler,it uses the median and IQR instead of the mean and std.

### 2. COlumn Transformer
When we have a dataset, it usually contains different types of features:
--Numerical features (e.g., Age, Salary, Temperature)
--Categorical features (e.g., Gender, City, Product Category)

Each type of feature often requires different preprocessing steps:
--Numerical → Scaling (StandardScaler, MinMaxScaler, RobustScaler, etc.)
--Categorical → Encoding (OneHotEncoder, OrdinalEncoder)

Instead of manually transforming each column and then concatenating them back together, ColumnTransformer lets you apply the right transformer to the right columns in one single object.
Its most helpful when we are making different data pipelines.



## Data Pipeline
A Pipeline is like a conveyor belt where 
We put raw data in at one end,
Each step (imputer → encoder → scaler → model) runs automatically,
and finally we get predictions or transformed data at the other end.
It makes sure everything is done in the correct order and that there’s no data leakage (using test data to influence training).

#### Advantages of using the pipelines
--its once built,can be reused with the help of the joblib
--can be integrated for the hyperparameter tunning like that in the gridsearchCV
--avoid the data leakage

