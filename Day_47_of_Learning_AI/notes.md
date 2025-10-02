welcome to my day 47/100 of Learning AI  

Today I am Learning the following topics  

# Feature Construction
-we do it using our domain knowledge and the intution and create new features.  
-it significantly improves the model performance.  

# curse of dimensionality
-we can call the features as the dimenaions of the data and sometimes more the dimensions bad  the performance of the model.  
-when we add the features to the data the model performance gradually becomes good but there is an optimum point and beyond that number of features there is no further improvement in the model performance.  
-the problem with the high dimension data is that it increases the sparsity.and as we know that most of the ML algorithms work on the basis of the statistics like the KNN that computes the distances and when the data is sparse then calculating the distances is not valid and the model performance gets very low.  
-but if the the model is performing well then in that case that is time and resource consuming as its causing the time and space complexity as the algorithm has to do more computations.  
 
## solution
reduce the dimesnionality by using the following ways.  

## Feature selection
-forward selection.  
-backward selection.  

## feature extraction
-PCA
-LDA
-tsne