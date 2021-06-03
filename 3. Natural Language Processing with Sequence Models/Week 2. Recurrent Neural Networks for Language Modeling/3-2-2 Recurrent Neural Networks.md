# Recurrent Neural Networks

Previously, we tried using traditional language models, but it turns out they took a lot of space and RAM.  For example, in the sentence below: 

![](EP3bxjHgQ6O928Yx4HOjhA_b12398ec1d6e474fb5756d84caf75b90_.png)

An N-gram (trigram) would only look at "did not" and would try to complete the sentence from there. As a result, the model will not be able to see the beginning of the sentence "I called her but she". Probably the most likely word is have after "did not". RNNs help us solve this problem by being able to track dependencies that are much further apart from each other. As the RNN makes its way through a text corpus, it picks up some information as follows: 

![](wJtPFB_DQXabTxQfw-F2vw_f9dd1fba8fad4f60a7bbab6df1ab22f6_.png)

Note that as you feed in more information into the model, the previous word's retention gets weaker, but it is still there. Look at the orange rectangle above and see how it becomes smaller as you make your way through the text. This shows that your model is capable of capturing dependencies and remembers a previous word although it is at the beginning of a sentence or paragraph. Another advantage of RNNs is that a lot of the computation shares parameters. 