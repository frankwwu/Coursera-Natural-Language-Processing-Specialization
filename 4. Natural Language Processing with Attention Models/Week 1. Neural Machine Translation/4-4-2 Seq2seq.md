# Background on seq2seq

Recurrent models typically take in a sequence in the order it is written and use that to output a sequence. Each element in the sequence is associated with its step in computation time tt. (i.e. if a word is in the third element, it will be computed at t_3. These models generate a sequence of hidden states h_t, as a function of the previous hidden state h_{t−1} and the input for position t. 

The sequential nature of models you learned in the previous course (RNNs, LSTMs, GRUs) does not allow for parallelization within training examples, which becomes critical at longer sequence lengths, as memory constraints limit batching across examples. In other words, if you rely on sequences and you need to know the beginning of a text before being able to compute something about the ending of it, then you can not use parallel computing. You would have to wait until the initial computations are complete. This is not good, because if your text is too long, then 1) it will take a long time for you to process it and 2) you will lose a good amount of information mentioned earlier in the text as you approach the end.  

Therefore, attention mechanisms have become critical  for sequence modeling in various tasks, allowing modeling of dependencies without caring too much about their distance in the input or output sequences. 
In this course, you will learn about these attention mechanisms and see how they are implemented. Welcome to Course 4! 

PS: Here's an article from The Atlantic that discusses the famous JFK speech containing the words "Ich bin ein Berliner," the example you saw in the Alignment video.

https://www.theatlantic.com/magazine/archive/2013/08/the-real-meaning-of-ich-bin-ein-berliner/309500/ (Putnam, 2013) 

