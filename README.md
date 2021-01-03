# Accuracy=79.99 %
# car-price-prediction
1.Data cleaning
2.Exploratory data analysis
3. Feature engineering
4. Feature selection
5. Model building
6. Performance of model
Converting Categorical Data to Numerical Data?
 This involves two steps:
Integer Encoding
# One-Hot Encoding
1. Integer Encoding
As a first step, each unique category value is assigned an integer value.

For example, “red” is 1, “green” is 2, and “blue” is 3.

This is called a label encoding or an integer encoding and is easily reversible.

For some variables, this may be enough.

The integer values have a natural ordered relationship between each other and machine learning algorithms may be able to understand and harness this relationship.

For example, ordinal variables like the “place” example above would be a good example where a label encoding would be sufficient.

2. One-Hot Encoding
For categorical variables where no such ordinal relationship exists, the integer encoding is not enough.

In fact, using this encoding and allowing the model to assume a natural ordering between categories may result in poor performance or unexpected results (predictions halfway between categories).

In this case, a one-hot encoding can be applied to the integer representation. This is where the integer encoded variable is removed and a new binary variable is added for each unique integer value.

In the “color” variable example, there are 3 categories and therefore 3 binary variables are needed. A “1” value is placed in the binary variable for the color and “0” values for the other colors.
# Exploratory data analysis
In data analysis we will Analyze to fnd out below stuff
a. Missing Value
b. Numerical variables
c. Categorical variables
d. Relationship between dependent and independent variables
# Feature engineering
a. Checking mutlicollinearity relation between variables and finding missing value too
b. Adding constant column in data
c. Feature scaling
d. converting categorical variables  into dummy variables
# Feature engineering
Splitting data into training and testing data
We use various method to find variables which are really healful in model building. 
a. use recursive feature elimination or lasso regression library for fueature selection.
split training and testing data into dependent and independent variables
# Model building
used ordinary least square method and linear regression for model building
# Accuracy and Perfornace of Model:
Find predicted value of model
r2score is used to to meassure accracy.
check p value that should be less than 0.05.
