
# Read 13
## Linear regression
-You know that linear regression is a popular technique and you might as well seen the mathematical equation of linear regression. But do you know how to implement a linear regression in Python?? If so don’t read this post because this post is all about implementing linear regression in Python. There are several ways in which you can do that, you can do linear regression using numpy, scipy, stats model and sckit learn. But in this post I am going to use scikit learn to perform linear regression.

-Scikit-learn is a powerful Python module for machine learning. It contains function for regression, classification, clustering, model selection and dimensionality reduction. Today, I will explore the sklearn.linear_model module which contains “methods intended for regression in which the target value is expected to be a linear combination of the input variables”.

-This data set is available in sklearn Python module, so I will access it using scikitlearn. I am going to import Boston data set into Ipython notebook and store it in a variable called boston.

-Scikit Learn

In this section I am going to fit a linear regression model and predict the Boston housing prices. I will use the least squares method as the way to estimate the coefficients.

Y = boston housing price(also called “target” data in Python)

and

X = all the other features (or independent variables)

First, I am going to import linear regression from sci-kit learn module. Then I am going to drop the price column as I want only the parameters as my X values. I am going to store linear regression object in a variable called lm.

-If you want to look inside the linear regression object, you can do so by typing LinearRegression. and the press <tab> key. This will give a list of functions available inside linear regression object.

-Residual plots are a good way to visualize the errors in your data. If you have done a good job then your data should be randomly scattered around line zero. If you see structure in your data, that means your model is not capturing some thing. Maye be there is a interaction between 2 variables that you are not considering, or may be you are measuring time dependent data. If you get some structure in your data, you should go back to your model and check whether you are doing a good job with your parameters.

