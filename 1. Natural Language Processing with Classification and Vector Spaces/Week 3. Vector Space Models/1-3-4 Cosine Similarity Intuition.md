# Cosine Similarity: Intuition

One of the issues with euclidean distance is that it is not always accurate and sometimes we are not looking for that type of similarity metric. For example, when comparing large documents to smaller ones with euclidean distance one could get an inaccurate result. Look at the diagram below:

![](t58dUAq9TUOfHVAKvZ1DnQ_96a1d23debfc4594b4283993af9b5a18_Screen-Shot.png)

Normally the food corpus and the agriculture corpus are more similar because they have the same proportion of words. However the food corpus is much smaller than the agriculture corpus. To further clarify, although the history corpus and the agriculture corpus are different, they have a smaller euclidean distance. Hence d_2 < d_1.

To solve this problem, we look at the cosine between the vectors. This allows us to compare \Beta B and \alphaα. 