# Word Embeddings

So why use word embeddings? Let's take a look.

![](hD4WFHuBS46-FhR7gfuOag_8b91201a0eda46f4bbac8e7a1b5b9f1b_Screen-Shot-2021-03-26-at-2.30.22-PM.png)

From the plot above, you can see that when encoding a word in 2D, similar words tend to be found next to each other. Perhaps the first coordinate represents whether a word is positive or negative. The second coordinate tell you whether the word is abstract or concrete. This is just an example, in the real world you will find embeddings with hundreds of dimensions. You can think of each coordinate as a number telling you something about the word. 

The **pros**:

* Low dimensions (less than V)
* Allow you to encode meaning