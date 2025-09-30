welcome to my day 37/100 of learning AI  
Today I am learning the following topics:  

## converting the numerical data into the catagorical
following are the two main techniques.  

## 1.descritization/binning
--bin is the alternative name for the interval.  
--process of transforming the continuous variable to the discrete by creating a set of contiguous variables that span the range of the variable's values.  
--it helps in reducing the outliers and  improve the data spread.  
### types:
--equal width/uniform binning(it can handle the outliers and the spread/distribution of the data remains same)  

--equal frequency/quantile binning(widh of each interval is not same.  its used more often as it improves the data spread and handles the outliers more effeciently.)  

--kmeans binning(its used when our data is spread in the form of the clusters.  it works on the base the kmeans algorithm)

### usage
-sklearn has the class named as kbinsdescritizer
## 2.Binarization