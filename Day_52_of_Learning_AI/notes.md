welcome to my day 52/100 of Learning AI
Today I am Learning the following topics

# Multiple Regression
 - when there are more than one columns in the features.  
 - extension of the simple LR.  
 - here we find the best fit plane in the 3D and hyperplane in 4D and onwards.  

 ![alt text](image.png)

![alt text](image-2.png)

- B1,B2 are weights means that they tell us how much is the role of that particalur column in predicting the output. 
- the Bo is the ouput and it ensures some value when all other paramaters are zero.  

- in the sklearn.datasets we have a class named as the make_regression() using which we can generate the dataset of our choice.  
- use the lr.coeff_ and lr.intercept_ on the lr trained object.  

## Mathematical formulation

![alt text](image-3.png)

![alt text](image-4.png)

![alt text](image-6.png)
then the y hat metrix becomes as:
![alt text](image-7.png)

y metrix is the target/prediction of all the values.  
B is the values of the coefficients.  
X is the metrix of all the input features.  i.e  
![alt text](image-8.png)
then we have
![alt text](image-9.png)
now we have
![alt text](image-10.png)
then
![alt text](image-11.png)
and now
![alt text](image-12.png)
to prove the equlaity of the mid terms we can do it as follow
![alt text](image-13.png)
![alt text](image-14.png)
now the original equation becomes as :
![alt text](image-15.png)
Here E is the loss function.  
![alt text](image-16.png)
![alt text](image-17.png)
![alt text](image-18.png)
![alt text](image-19.png)


- as we discussed above the simple and the multiple LR uses the OLS method(some specific formula) that finds the values. but in this method(as we can see the above formula) we have to do lot of the computations that slows down the algorithm .  
- solution is the gradient desent where we use the approximation instead of the exact values.  
- SGDRegressor is the class of the sklearn for the linear regression that uses the  gradient descent method in the backend.but its used when the data is extremely higher dimension.  