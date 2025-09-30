welcome to my day 39/100 of learning AI  

Today I am learning the following topics  

# Handling the missing data
--we can remove the whole row of the missing data(but its not most preferable) 
--we can impute them i.e fill them and can be univariate or the multivariate

### imputation

#### univariate 

for catagorical data-  
---use the mean/median/some random value etc.  

for the numerical data use mode etc.  

#### multivariate
use the :  
--KNN imputer  
--iterative imputer  



# Complete case analysis(CCA)

-removing the missing values  
-also known as the list-wise deletion  
-this focuses on the idea that work only on those rows having the complete data.  

### assumptions for the CCA
-values are missing completely randomly.(MCAR)  
-if the data is MCAR then it preserves the variable distribution.  

### disadvantages
--it can affect the distribution of the data if not the MCAR.  
--when using the model in production, then model don't know how to handle the missing data.  

### when to use?
-if data is MCAR.  
-if the missing data is <5% then can apply it .in case of more don't apply it.  

