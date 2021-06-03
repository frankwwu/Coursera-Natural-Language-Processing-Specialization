# Neural Networks for Sentiment Analysis

Previously in the course you did sentiment analysis with logistic regression and naive Bayes. Those models were in a sense more naive, and are not able to catch the sentiment off a tweet like: "I am not happy " or "If only it was a good day". When using a neural network to predict the sentiment of a sentence, you can use the following. Note that the image below has three outputs, in this case you might want to predict, "positive", "neutral ", or "negative". 

![](rZuVhCYrRPublYQmK5T7pw_d74292138bab40eda582b67fd54767ae_Scree.png)

Note that the network above has three layers. To go from one layer to another you can use a WW matrix to propagate to the next layer. Hence, we call this concept of going from the input until the final layer, forward propagation. To represent a tweet, you can use the following: 

![](72QwSjMSR1ykMEozErdcqQ_f32099253b934aaaac7a496b07e9020a_Screen-Sh.png)

Note, that we add zeros for padding to match the size of the longest tweet. 