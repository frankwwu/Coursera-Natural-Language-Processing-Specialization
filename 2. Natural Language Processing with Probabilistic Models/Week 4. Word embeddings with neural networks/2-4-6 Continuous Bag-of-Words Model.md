# Continuous Bag of Words Model

To create word embeddings, you need a corpus and a learning algorithm. The by-product of this task would be a set of word embeddings. In the case of the continuous bag-of-words model, the objective of the task is to predict a missing word based on the surrounding words.

![](o744WuCZQO6-OFrgmfDuJA_91f4eb4536a347a089e17d654d296947_Screen-Shot-2021-03-29-at-9.24.15-AM.png)

Here is a visualization that shows you how the models works.

![](_84SgGXiSNSOEoBl4rjUxw_537e5eb6ce7e49cdac4f3adccb702fde_Screen-Shot-2021-03-29-at-9.26.34-AM.png)

As you can see, the window size in the image above is 5. The context size, C, is 2. C usually tells you how many words before or after the center word the model will use to make the prediction. Here is another visualization that shows an overview of the model. 

![](IgFIDDSeRTWBSAw0nmU1fg_a466dc9d154649b1a5c1f85cabc7799a_Screen-Shot-2021-03-29-at-10.28.27-AM.png)