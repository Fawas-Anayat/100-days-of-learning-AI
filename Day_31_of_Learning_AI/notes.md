welcome to my day 31/100 of learning AI

# Feature scaling
standardize the range of the independent variables to a range so that certain ML algortihms don't confuse and get the uncertain results

## types
## 1.standardization(also called as the z-score normalisation)
-->we set the values as the mean=0 and the std=1
--> can be done using the standardcaaler from the preprocessing of the sklearn
-->standardscaler takes the dataframe as an input but returns the numpy array
-->Distribution of the data before and after it remains same 
-->will it make the performance of the model better ? it depends on the algorithm like it will significantly increase the accuracy of the logistic regression but won't affect the decisiontree accuracy 
---> the outliers in the data won't be reduced using it .their effect will be same.rather we have to reduce them explicitely
-->we can use it when working with the following algorithms:
        -->kmeans
        -->knn
        -->pca
        -->aritificaial neural networks
        -->gradient descent 
--> dont use it in the following algorithms
        -->tree based algorithms
        -->random forest
        -->decision tree 
        -->gradeint boost
        -->xgboost

## 2.normalization