welcome to my day 48/100 of Learning AI

Today I am Learning the following topics  

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