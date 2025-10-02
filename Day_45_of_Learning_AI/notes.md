welcome to my day 45/100 of Learning AI

Today I am Learning the following topics  

# outliers
-outliers are not always dangerous and we need to decide it very carefully that whether to remove them or keep them.  

## outliers affect which algorithms
they affect those algorithms that calculates the weight of the values,like:  
-linear regression  
-logistic regression  
-adaboost  
-deep learning  

they don't affect the tree based algorithms.  

## how to remove the outliers:
### 1.trimming
we completely remove the outliers but the issue with this technique is that it thins the data.  

### 2.capping
we put limit that the value below this range is outlier and assign a specific value to the values below that range.  

### 3.other techniques
-treat them like the missing values.  
-discritization.  


## how to detect the outliers:

### 1. normal distribution
if the data is in the form of the normal distribution then we know that the 99% data is present in mean +3 std away and any value beyond this range is considered as the outlier.  

### 2. skewed distribution
if the data is skewed then we can use the box plot to check the values beyond from the minimum and maximum value.  

### 3. other distribution:
we can consider that the values beyond the 99th percentile and the values below 5 percentile is outlier.  

