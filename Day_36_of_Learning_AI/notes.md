welcome to my day 36/100 of learning AI  
Today I'll be learning the following topics

## mathematical transformations
## transformers in the sklearn:
1--function transformer have the log ,reciprocal,costum transformtions  
2-->power transformers have the box cox and the xeo johnson transformers  

--After these transformtion the model performance gets improved  
--some ML algortihms performs well on the normal distribution while others don't
--They convert the distribution of the data to the normal  

#### How to find out the data is normal?
--sns.displot  
--pd.skew()  
--QQ plot--in the qq plot if the data points are as a line in the 45 degree angle then its the normal  
### 1.log transformation
--we simply take the log of all the values and the data  becomes the normally distributed  
--dont work on the negative values  
-- when we apply on the right skewed data then that data gets normal  
-- the data gets distributed linearly and therfore the performance of the linear models gets better after it  

### 2.reciprocal transformation

### 3.square transformation
--applied on the left skewed data
### 4.square root transformation