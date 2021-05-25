# Bayes' Rule

Conditional probabilities help us reduce the sample search space. For example given a specific event already happened, i.e. we know the word is happy:

![](xoYzIfcHT0uGMyH3B69LQw_3b10c11c4a504416b8ea133f0c97.png)

Then you would only search in the blue circle above. The numerator will be the red part and the denominator will be the blue part. This leads us to conclude the following: 

![](gXRnWNLHSOy0Z1jSx3jscg_b2c28038bf054638a38ef02a1ac7.png)

Substituting the numerator in the right hand side of the first equation, you get the following: 

![](0Jl5aETpQImZeWhE6bCJrg_5d5d25924694451fa3eae308da64.png)

Note that we multiplied by P(positive) to make sure we don't change anything.  That concludes Bayes Rule which is defined as 

P(X|Y) = \frac{P(Y|X) P(X)}{P(Y)}.
 