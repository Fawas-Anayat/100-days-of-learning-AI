welcome to my day 40/100 of learning AI  

Today I am learning the following topics  

# imputing the numerical data
## 1.univariate imputation
## 1.mean/median imputation  
--> use mean if the distribution is normal.  
-->use median if the distribution is skewed.  
--after the mean/median imputation the variance changes.  
--use the class of the sklearn named as the SimpleImputer.  

## disadvantages
-it changes the shape of the distribution.  
-there comes outliers 
-change in the covariace/correlation  

## when to use:
-MCAR  
-missing values < 5%  


## 2. arbitrary imputation
-use some arbitrary values to replace the missing values.  
-it can be used in both the numerical as well as the catagorical data.  
-used when there is no MCAR.
-not widely used as there are other techniques that are more viable.  

## 3.End of distribution imputation
-same to the arbitrary but here we don't take the random value instead we take some value from the end of the distribution i.e outlier.  
-use when data is not MCAT.  
