welcome to my day 33-35/100 of learning AI  
Here I am learning the following topics  


## simple imputer
fills the missing values in the column and can be filled using different techniques like the mean or the most frequent values


## column transformers
--handling all the columns of the different datatypes easiy
--its present in the sklearn
--we pass the list of tuples in it
-->import the columntransformer class from sklearn.compose it has the paramters like transformers in which we have to write the names of the encoders etc and all the details inside them like the columns names etc and there is a parameter at the end named as the remainder that tells what to do with the remaining columns and we can write drop if want to delete the remaining columns and can write the passthrough if want to keep the remaining columns
--the best stretegy is that call the columns by their index numbers not the names as these tranformers returns the np arrayst that have no names of the columns

## sklearn pipelines
--> chains together differnt steps so that the output of one step is used as the input in the next step
-->helps to apply the same preprocessing steps to the train and test data
-->pipeline class(you have to pass a list of the tuples and write the details about the column transformers) vs make_pipline function(just pass the names of the column transformers) and the same logic is applied in the case of the transformer and the make_transformer