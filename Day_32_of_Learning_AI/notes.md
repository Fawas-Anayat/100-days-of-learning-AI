welcome to my day 32/100 of learning AI
Today I will be learning these topics

## Encoding catagorical data
as the ML algorithms deals with the numeical data but the catagorical data is in the form of the strings therefore we have to convert them into the numbers before feeding into the ML algorithm

## types
## 1. ordinal encoding 
-->applied on the ordinal data  
-->we apply it only on the input features of the data that will be given to the ML algorithm  
--> for the ouput / target column of the data that is used in the classification algorithms we use the label encoders that is specially designed for the label column  

## 2.nominal encoding 
-->used on the nominal catagorical data  
-->used the onehot encodor in this case.  
-->we can say that there are vectors formed of the catagorical data that shows the presence or absence of some feature in a column.  
--> when there are many catagories in a dataset then we should apply the OHE only on the most frequenct catagories and combine the others to a single column like with the name others and in this way we can reduce the dimensionality  
-->for the onehot encoding we also have a function in the pandas named as the get_dummies apart from the one in the scikit learn but its not so much efficient

### dummy variable trap
after the one hot encodor applied there are many columns of the catagorical data that somehow raises a mathematical raltion between the column which is called as the multi collinearity which is curse for the linear models as in their case we assume all the input columns as the independent.  
to solve this problem we simply delete one column and hence the multicollinearity is broken
