# Training / Testing

After preparing the batches of vectors, you can proceed to multiplying the two matrices. Here is a quick recap of the first step: 

![](Bo4Dh2kITm-OA4dpCN5vLw_899efb44b116440baf003b893ec94c8d_Screen-Shot-2021-04-13-at-3.40..png)

The next step is to implement the siamese model as follows: 

![](V-18lhYVTaatfJYWFc2mcw_bab3257b36ea49bd95f2a37ef6e40c34_Screen-Shot-2021-04-13-at-3.41..png)

Finally when **testing**: 

* Convert two inputs into an array of numbers
* Feed it into your model
* Compare 𝒗1,𝒗2 using cosine similarity
* Test against a threshold \tauτ