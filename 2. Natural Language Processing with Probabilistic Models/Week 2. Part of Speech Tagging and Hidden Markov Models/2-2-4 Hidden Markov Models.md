# Hidden Markov Models

In the previous video, I showed you an example with a simple markov model. The **transition probabilities** allowed you to identify the transition probability from one POS to another. We will now explore hidden markov models. In hidden markov models you make use of **emission probabilities** that give you the probability to go from one state (POS tag) to a specific word. 

![](DkG3PmJgRRaBtz5iYCUW-Q_0ac536e5ad5946d1976fd2d6274d1907_Screen-Shot-2021-03-10-at-12.23.16-PM.png)

For example, given that you are in a verb state, you can go to other words with certain probabilities. This emission matrix **B**, will be used with your transition matrix **A**, to help you identify the part of speech of a word in a sentence. To populate your matrix **B**, you can just have a labelled dataset and compute the probabilities of going from a POS to each word in your vocabulary. Here is a recap of what you have seen so far: 

![](DeQr3EW3RRWkK9xFt-UVeA_3c043c978f22429a9fa653ef6b87d9b0_Screen-Shot-2021-03-10-at-12.36.48-PM.png)

Note that the sum of each row in your **A** and **B** matrix has to be 1. Next, I will show you how you can calculate the probabilities inside these matrices.
