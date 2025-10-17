welcome to my day 56-65/100 of Learning AI  

Today I am learning the gradient descent

# Gradeint Descent
- optimization algorithm.  
- when we give it any differentiable function,it returns us the minima.  
- used in many ML algorithms like the linear and logistic regression and is the backbone of the deep learning.  

we are going to understand it while applying it on the linear regression.  

## Mathematical Intuitiom
Look at the ss below,  

![alt text](image.png)
Unlike the OLS where we can easily find the value of the b if we put the loss function equal to zero and then differentiat it.  
Here we have to go to the minimum value and for this purpose we have to first find the direction where the minimum is located ,so we can differentiate it which can help us find the slope.  now we can infer the result as follow:
- if the value of the slope is negative this means that we have to go forward i.e increment the value of the b to go to the minimum.  
- if the slope is positive then we have to go backward i.e decrrement the value of the b to go to the minimum.   
- the equation for the new value of the slope becomes as follow .  

![alt text](image-1.png)

as we see in the above equation , we observe very drastic changes in the value of the b and its often the zig zag pattern of the graphs in the function graph. this large learning rate can cause the skipping of the actual solution. To overcome this issue we can take a new variable named as the learning rate.  i.e   

![alt text](image-2.png)

the value of the learning rate can be any depending upon our condition.  

### when to stop
its an iterative algorithm so getting to know when to stop is important which can approached as following.  
- find the difference of the b_new and the b_old and if its very small(<0.0001) then it means we have reached our desired solution,  
- we can set the iterations to a specific numbers like 100 or 1000. these no of iterations is known as the epochs.we can find the no of epochs easily while looking at the graph .  


after done with the mathematical intuition above we can now use the exact mathematical formulation as below.  


## Mathematical Formulation
Look at the following ss.we can infer that we have to find the value of the slope by finding the derivative at that specific condition.  
![alt text](image-3.png)
and in this way we get the value of the slope and we find it again iteratively untill at the end we get the minimum value which is our requirement.  
- learning rate multiplied by the slope is termed as the step size.  

- we are calculating the gradient and thats why its known as the gradient descent.  
![alt text](image-4.png)



