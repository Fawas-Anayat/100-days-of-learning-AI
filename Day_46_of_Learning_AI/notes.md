welcome to my day 45/100 of Learning AI

Today I am Learning the following topics  


#  outlier detection and removal using the Z-score
-this method is implemented on the normal distribution only.  
-after we detected the outler we can trim or cap them.  

# outlier detection and removal using IQR
-used when the data is a little skewed.  
-values beyond the whiskers in the box plot are said to be the outliers.  
-the whiskers can be calculated using the IQR-proximity rule.  

(quick update--the np.where() function of the numpy..we pass three arguments in it that are np.where(condition,what_to_do_if_its_true,what_to_do_if_its_false))

# outlier detection and removal using the percentile method
-we set a threshold that the value below and above that threshold percentile is the outlier.  
- we can use the df.quantile(some value) function of the pandas to find the right percentile values.  
-to remove we can simply do the trimming or the capping.  
-capping in this technique is known as the winsoriztion.  
