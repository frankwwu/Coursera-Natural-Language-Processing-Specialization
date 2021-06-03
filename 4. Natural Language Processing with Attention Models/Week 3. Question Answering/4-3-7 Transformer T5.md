# Transformer T5

One of the major techniques that allowed the T5 model to reach state of the art is the concept of masking:

![](o4imCe3yRIyIpgnt8mSMqQ_4b9b5e226a0146d9b3a342a2c714db81_Screen-Shot-2021-01-22-at-2..png)

For example, you represent the “for inviting” with &lt;X&gt; and last with &lt;Y&gt; then the model predicts what the X should be and what the Y should be. This is exactly what we saw in the BERT loss. You can also mask out a few positions, not just one. The loss is only on the mask for BERT, for T5 it is on the target. 

![](t01efIy9TfmNXnyMvV35mQ_57df2fc594c04b45a78f46e77466f9d0_Screen-Shot-2021-01-22-at-2..png)

So we start with the basic encoder-decoder representation.  There you have a fully visible attention in the encoder and then causal attention in the decoder.  So light gray lines correspond to causal masking. And dark gray lines correspond to the fully visible masking. 

In the middle we have the language model which consists of a single transformer layer stack. And it's being fed the concatenation of the inputs and the target. So it uses causal masking throughout as you can see because they're all gray lines. And you have X1 going inside, you get X2, X2 goes into the model and you get X3 and so forth. 

To the right, we have prefix language model which corresponds to allowing fully visible masking over the inputs as you can see with the dark arrows. And then causal masking in the rest.