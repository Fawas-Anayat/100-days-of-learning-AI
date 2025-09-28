welcome to my day 33-35/100 of learning AI  
Here I am learning the following topics  

## column transformers
--handling all the columns of the different datatypes easiy
--its present in the sklearn
-->import the columntransformer class from sklearn.compose it has the paramters like transformers in which we have to write the names of the encoders etc and all the details inside them like the columns names etc and there is a parameter at the end named as the remainder that tells what to do with the remaining columns and we can write drop if want to delete the remaining columns and can write the passthrough if want to keep the remaining columns

## sklearn pipelines
--> chains together differnt steps so that the output of one step is used as the input in the next step
-->helps to apply the same preprocessing steps to the train and test data