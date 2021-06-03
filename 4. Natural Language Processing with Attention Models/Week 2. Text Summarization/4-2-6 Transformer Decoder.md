# Transformer Decoder

That was a lot of information! Don't worry if you did not understand everything, we will go over everything step by step. 

![](Q0Awy7SQQGGAMMu0kJBhvg_ddb63a5431f34ea283157ab576068473_Screen-Shot-2021-01-04-at-2..png)

Once you get the embeddings, you append to it the positional encoding, which you can think of just a learned number that tells you information about the position of the word. Then, you do mutli-head attention as explained in the previous video/reading. There is a feedforward layer with a ReLU after, a residual connection with layer normalization (repeat the block shown above N times), finally a linear layer with a softmax. Zoning into the block that gets repeated N times, you get the following: 

![](AWvNFeRPSYerzRXkT3mHQA_6295964754f74643814e49622f13869d_Screen-Shot-2021-01-04-at-3..png)

Now for the feedforward block, you can just implement the following: 

![](fSGJxX3xQAmhicV98RAJhg_71c31437b4464c9c81ee8aaa2efb1a97_Screen-Shot-2021-01-04-at-3..png)

You get the input, (red vector) run it through self-attention and then a feedforward with ReLU. At the end of the decoder, you can just run a softmax.


