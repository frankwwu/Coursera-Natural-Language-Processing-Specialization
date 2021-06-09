# BERT Objective

We will first start by visualizing the input. 

![](n8pn0zAVSMWKZ9MwFajFxw_7c6a1a1e5d9f40699906e36b52e215db_Screen-Shot-2021-01-22-at-12.png)

The input embeddings are the sum of the token embeddings, the segmentation embeddings and the position embeddings.

**The input embeddings**: you have a CLS token to indicate the beginning of the sentence and a sep to indicate the end of the sentence

**The segment embeddings**: allows you to indicate whether it is sentence a or b.

**Positional embeddings**: allows you to indicate the word's position in the sentence.

![](vDlfRa8ySIu5X0WvMkiLYg_f1c15b19773d470cae64ddb8c6bccaac_Screen-Shot-2021-01-22-at-12.png)

The C token in the image above could be used for classification purposes. The unlabeled sentence A/B pair will depend on what you are trying to predict, it could range from question answering to sentiment. (in which case the second sentence could be just empty). The BERT objective is defined as follows: 

![](PGZpKHWbRI6maSh1m_SO6w_c950e9a0c9c946e5b2c95aa0049eed6e_Screen-Shot-2021-01-22-at-12.png)

You just combine the losses! 

