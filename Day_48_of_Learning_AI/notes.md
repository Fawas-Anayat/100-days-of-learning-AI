welcome to my day 48/100 of Learning AI

Today I am Learning the mathematical foundation of the PCA in depth and detail and all the notes are here in this file.

-spread is not the variance exactly.  
-variance is proportional to spread.  
-in PCA we take the variance instead of the mean absolute deviation as the mode function is not diffrentiable at zero while the sqaure function of the variance is very good differentiable at zero.  

# PCA
-reduces the dimensions of the data by keeping the real essence of the data.  
-when we are manually selecting the faetures then we can plot two features and will select that features  that has more spread on the corresponding axis i.e variance of the data.  
-but if its the same means(means the variance is same on all the features) that the label value depends greatly on both the features . then in that case we can't do the manual removal of the features and here we need the PCA and we have ro reduce the dimesion instead of deleting the features manually.  
-PCA forgets the old features of the dataset and creates the new ones on the basis of that old features.  
-PCA  shifts the axes and new axes are formed(known as the principal components) and we now again check the variance on the basis of that new axes.
-the simple idea is that PCA transforms the axis such that to maximize the variance on some axes.     
        no of PCs <= no of total features 


## why variance is imp in pca?
-as the relation between the points is often shown by the distance between them and if we convert the data from the higher dimension to the lower dimension then to preserve that distance we take the axes that have the maximum spread , if we take the minimum spread then we'll have no idea of the relation of the points of ths data.  


## mathematical  problem formulation of pca
we consider each data point as the vector and find the projection of each point on a unit vector and that projection gives us a scaler quantity that is simply the distance of that point on the unit vector.  
now we have to choose that unit vector for which the variacnce is maximum.  

-the core idea is that we will check the variance of the projections on lot of unit vectors and then select that unit vector for which the variance is maximum. 
-we can say that its the optimization function.   

#### covariance
tells the relation between two features.its values can be any, positive to negative.  

#### corelation
same as the covariance but its values are restricted between 0 and 1.  

#### covariance  metrix
-its a sqaure metrix.  
-its a symmetrical metrix where the diagonal elemsnts are the variance of each column and and the non diagonal are the covariance.  
-it tells the spread of each and every axis.  
-it tells the relationship/covariance between all the axes.  


## matrices
-matrices are the linear transformations. They when applied to a coordinate system all of its points are transformed.  
-identity metrix when applied to a coordinate system it don't change/transform the values so thats a special case and therefore its known as the identity metrix.  
-they,when applied, change the orientation of the cartesian coordinate system(where each point/number can be treated as the vector) and then the magnitudes as well as the direction of the points/vectors gets changed.  
-geogebra is the tool/website through which we can find the transformations.  

### eigen vectors
-a special vector and their direction don't change upon transformation ,instead their magnitude can be changed.   
-when we apply the linear transformation to a 2-D coordinate system we get minimum two eigen vectors.  
-in 3D are three eigen vectors and so on.  

### eigen values
- as the eigen vector don't change its direction upon the linear transformation but its can change its scale/magnitue.  
- this change in the scale / magnitude is known as the eigen value.  
-its the the factor with which the eigen vector changes its scale.  

## final points about the metrices
when we find the eigen values of the covariance metrix then the eigen vector having the highest eigen value is the one that points in the direction of the highest variance.  
-the eigen vector having the highest eigen value is the PC1 ,2nd highest is the PC2 and the third highest is the PC3.  
-when we get the principal components we transform the points from n-d to the 3d ,2d or any dimension as we wish.  


# how pca works?
- make the data as the mean centerd.it improves the performance of the pca.  
- find the covariance metrix.  
- find the eigen vectors and eigen values.  
- transform all the data points to the new dimension as we wish.  

-these all functions can be applied easily using the sklearn.

## pca using the sklearn
- use the pca class of the sklearn  
- in the pca object there is a keyword argument that is n_components that shows the number of PCs we want to draw.  
- some benefits with  the pca trained object are the arguments like pca.explained_variance_ that shows us the eigen values.  
- and the pca.components_ gives us the eigen vectors.  


## how to find the optimum number of the PCs:
- a single eigen value tells us that how much its corressponding eigen vector explains the variance of the data.  
- we find the percentage of the eigen values and then take that amount of the eigen vector so that we can easily explain at least 90 % of the variance of the data.  
- use the pca.explained_ratio_ for getting the %.  
- use this for the graph..plt.plot(np.cumsum(pca.explained_variance_ratio_))


## when pca won't work
- when the data is circular format means the variance on the x axis and the y axis is same.  
- when the data has some special form in the higher dimension like the sine curve then don't appply the pca as it won't preserve that pattern in the lower dimension.  
 