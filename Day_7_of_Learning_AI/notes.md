Welcome to my day 7/100  of Learning AI
Today I am exploring the topics that were left tomorrow about the data preprocessing.

### 1. OrdinalEncodor
OrdinalEncoder converts ordered categorical features (like Low < Medium < High) into integers that preserve the order:
Low -> 0
Medium -> 1
High -> 2
This is different from OneHotEncoder (which makes separate 0/1 columns and does not imply order). Use Ordinal only when the categories truly have an order.
If the data don't have the natural order,then don't use the ordinalencodor,instead use the onehotencodor