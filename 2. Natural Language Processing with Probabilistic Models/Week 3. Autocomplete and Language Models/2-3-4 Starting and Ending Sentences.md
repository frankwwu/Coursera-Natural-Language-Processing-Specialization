# Starting and Ending Sentences

We usually start and end a sentence with the following tokens respectively: &lt;s&gt; &lt;/s&gt;. 

When computing probabilities using a unigram, you can append an &lt;s&gt; in the beginning of the sentence. To generalize to an N-gram language model, you can add N-1 start tokens &lt;s&gt;. 

For the end of sentence token &lt;/s&gt;, you only need one even if it is an N-gram. Here is an example: 

![](vWvZ_75GQ0ur2f--RrNLTQ_165f10835c93464687bb934d3ab3d522_Screen-Shot-2021-03-24-at-12.23.32-PM.png)

Make sure you know how to compute the probabilities above! 
