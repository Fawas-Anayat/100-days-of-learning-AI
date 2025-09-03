Welcome to day 6/100
Today I started by learning how can i make a data pipline and then statrted exploring different methods i can transform data .
These transformations are not just like that of the data cleaning in the pandas but it invloves different statistical concepts

# Data Pipeline
Its a series of steps though which raw data is passed to make it clean and able to be used by machine learning model for model training

#### Data pipeline in scikit-Learn
following is the syntax for the data pipline in sckit-Learn:
from sklearn.pipeline import Pipeline

pipeline = Pipeline(steps=[
    ('step_name_1', transformer_1),
    ('step_name_2', transformer_2),
    ...
    ('estimator', model)
])

In the sk pipline,we must have all the transformers in the first and the last one must be the esimator

##### Transformer
Means it transforms the data into some new shape .i can be implemented using fit and transfom methods
eg:SimpleImputer,StandardScaler,OneHotEncoder,PCA

##### Estimator
It predicts some new value based on learning from the old data
eg:LogisticRegression, RandomForestClassifier, LinearRegression



##### following are some of the major transformers and their functions
### 1. simple imputer
handles the missing values in the dataset.The missing value can be replaced by the mean,median,most frequent value and can also be a constant value.we can also add a feature so that it will add a new column in the dataset that has the boolean value and the value will be true for the sample where there is a missing value

### 2.standardscaler
standardize the numerical values in the  data so that the mean =0 and the std=1. This puts the features on the same scale   
Its not a good choice if there are lot of outliers in the dataset.For such case we use the robust scaler that uses the mean and IQR

--imp point for making a histogram from a dataframe containing more than one features
scaled_df.hist() → multiple subplots, 1 per feature.
scaled_df.plot(kind="hist") → single plot, all features overlaid.

### 3.OneHotEncodor
transforms the catagorical data into the binary form
instead of giving the 1,2,3.. numbers to the catagorical variables,it creates a completely new column that shows the presence(1) or absence(0) of that variable in that column
standardscaler is for the numerical data and the onehotencoder is for the catagorical data

### 4.MinMaxScaler
scales numerical data into a small range of intervals like between 0 and 1
--its sensitive to the outliers
--always fit the scaler on the training data and only transform it on the test data to avoid the data leakage 
--minmaxscale does not affect the distribution or spread of the data

### 5. OrdinalEncodor

### 6.ColumnTransformer


