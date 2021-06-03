# Dot-Product Attention

Dot product attention could be summarized as follows:

![](YuNRwDQYRSOjUcA0GCUjig_db064a6cf3574f0f882cbfa1723d0290_Screen-Shot-2020-11-06-at-3..png)

Given an input, you transform it into a new representation or a column vector. Depending on the task you are working on, you will end up getting queries, keys, and values. Each column corresponds to a word in the figure above. Hence, when you compute the following: 

![](pyLYbsxDRrWi2G7MQ9a1Vg_8a7300b8ba134f9f81f22272d04c8701_Screen-Shot-2020-11-06-at-3..png)

This concept implies that similar vectors are likely to have a higher score when you dot them with one another. You transform that score into a probability by using a softmax function. You can then multiply the output by VV. 

![](A2FQsFMkTFahULBTJNxWnw_85f7d9549119422d95a0ea17c4262dc5_Screen-Shot-2020-11-06-at-3..png)

You can think of the **keys** and the **values** as being the same. Note that both K, V are of dimension L_k, D. Each query q_i picks the most similar key k_j. Queries are the German words and the keys are the English words. Once you have the attention weights, you can just multiply it by V to get a weighted combination of the input. 
