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



