# Logistic Regression Overview

Logistic regression makes use of the sigmoid function which outputs a probability between 0 and 1. The sigmoid function with some weight parameter \theta and some input x^{(i)} is defined as follows. 

![](oL4Ox_JxTBi-DsfycUwYvw_d0582a0dddf7470486f0.png)

Note that as \theta^Tx^{(i)} gets closer and closer to -\infty the denominator of the sigmoid function gets larger and larger and as a result, the sigmoid gets closer to 0. On the other hand, as \theta^Tx^{(i)} gets closer and closer to \infty the denominator of the sigmoid function gets closer to 1 and as a result the sigmoid also gets closer to 11. 

Now given a tweet, you can transform it into a vector and run it through your sigmoid function to get a prediction as follows: 

![](THV0BbogT2i1dAW6IA9oMg_67bcc86617b54ac4b575.png)
