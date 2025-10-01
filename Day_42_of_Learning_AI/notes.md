welcome to my day 42/100 of Learning AI  

Today I am learning the following topics  

# Random imputation

-select some random numbers from the data and fill the missing values with that random numbers.  
-distribution of the data remains same.  
-covariance in the data is disturbed as we are introducing the randomness in the data .  
-use this technique when we are going to apply this data to the linear models and it won't work well on the tree based algorithms.  
-memory heavy for the deployment.  
-we can implement this technique using the pandas.  

# Misssing indicator
-for each column we create a new one and in that column we write true for the missing value and false for the non-missing values.  
-surprisingly this technique sometimes makes model perform well.  
-there is class named as the missing indicator in the sklearn for this.  
-in the simpleimputer class there is a paramter named as "add_indicator" which if kept true it can act as the missing indicator and we won't need to call separately the missing indicator class.  
-this parametr is also present in the knnimputer and in the iterativeimputer.  
