#  Architecture of the CBOW Model Activation Functions

## ReLU funciton

The rectified linear unit (ReLU), is one of the most popular activation functions. When you feed a vector, namely x, into a ReLU function. You end up taking x = max(0, x). This is a drawing that shows ReLU. 

![](fSqzc6nHRD6qs3OpxzQ-sA_2f7c9fdebc1b4cbcb7baa601615a28ee_Screen-Shot-2021-03-29-at-2.04.42-PM.png)

## Softmax function

The softmax function takes a vector and transforms it into a probability distribution. For example, given the following vector z, you can transform it into a probability distribution as follows. 

![](SxzQIC97S2ec0CAve9tn-g_e7ee1f7b8e384c96836413270dd6c0b7_Screen-Shot-2021-03-29-at-2.09.36-PM.png)

As you can see, you can compute \hat y = \frac{e^{z_i}}{\sum_{j=1}^V e^{z_j}}.
