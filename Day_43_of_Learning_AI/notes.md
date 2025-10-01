welcome to my day 43/100 of Learning AI  

Today I am learning the following topics

# Multivariate missing value imputation

-here we use more than one columns so that we can easily fill the values of a column while in the univariate imputation we just use the single column values to fill the missing values in that column.. 

## types
### KNN imputer
-works on the basis of the KNN algorithm.  
-where we find the eucledian distances from that missing value to the nearest neighbours and then keep the number of neighbours that are given by the k.AFter that we find the mean of all the values in that KNN and fill the missing value by it.  
-if the neighbour rows also have the missing values we use the nan-eucledian distances which can easily handle the missing values also.  

#### final points
-KNNimputer is more accurate means it gives better results.  
-there are large number of calculations as we are calculating the distances for large number of values.  
-memory inefficient --as when we deploy the model on the server we have to put all the x train data on the server also as when the model faces the new data it will calculate the distances from all the points in the training data.  
-use the KNNimputer class of the sklearn.  
