# Basic Word Representations
Basic word representations could be classified into the following:

* Integers
* One-hot vectors
* Word embeddings

![](p1ISbqzJTtWSEm6syS7VlQ_47c983d709ef48e193082828b054ce46_Screen-Shot-2021-03-26-at-2.15.25-PM.png)

To the left, you have an example where you use integers to represent a word. The issue there is that there is no reason why one word corresponds to a bigger number than another. To fix this problem we introduce one hot vectors (diagram on the right). To implement one hot vectors, you have to initialize a vector of zeros of dimension V  and then put a 1 in the index corresponding to the word you are representing.

The **pros** of one-hot vectors:  simple and require no implied ordering. 

The **cons** of one-hot vectors: huge and encode no meaning. 

 