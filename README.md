# Normalization-RegularizationTechniques

This repository contains datasets with 5 different Normalization and Regularization Techniques combined

#Normalization:
Normalization is a technique often applied as part of data preparation for machine learning. The goal of normalization is to change the values of numeric columns in the dataset to use a common scale, without distorting differences in the ranges of values or losing information. Normalization is also required for some algorithms to model the data correctly.

#Regularization: 
Regularizations are techniques used to reduce the error by fitting a function appropriately on the given training set and avoid overfitting.Also, some techniques of regularization can be used to reduce model parameters while maintaining accuracy,
for example, to drive some of the parameters to zero.

This might be desirable for reducing the model size or driving
down the cost of evaluation in a mobile environment where processor power is constrained.

We have 2 different Regularization Techniques:
L1 or Lasso Regularization:
#L1 regularization:
It adds an L1 penalty equal to the absolute value of the magnitude of coefficients.
When our input features have weights closer to zero this leads to sparse L1 norm.
In the Sparse solution, the majority of the input features have zero weights and
very few features have non zero weights.

Features:
L1 penalizes the sum of the absolute value of weights.
L1 has a sparse solution
L1 generates a model that is simple and interpretable but cannot learn complex patterns
L1 is robust to outliers

#L2 Regularization:
L2 regularization is similar to L1 regularization.
But it adds a squared magnitude of coefficient as penalty term to the loss function.
L2 will not yield sparse models and all coefficients are shrunk by the same factor
(none are eliminated like L1 regression)

Features:
L2 regularization penalizes the sum of square weights.
L2 has a non-sparse solution
L2 regularization is able to learn complex data patterns
L2 has no feature selection
L2 is not robust to outliers


There are 5 cases models were trained on
1. L1 Regularization with Batch Normalization
2. L2 Regularization with Batch Normalization
3. L1 & L2 Regularization with Batch Normalization
4. Ghost Batch Normalization (GBN)
5. L1 & L2 Regularization with GBN
