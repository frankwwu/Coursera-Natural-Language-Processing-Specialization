# Evaluation for Machine Translation

The closer the BLEU score is to one, the better your model is. The closer to zero, the worse it is. 

To get the BLEU score, the candidates and the references are usually based on an average of uni, bi, tri or even four-gram precision. To demonstrate, I'll use uni-grams as an example. Look at the following table:

![](kh3QCN8UR22d0AjfFOdtrQ_41c0c74a9b9e4be19ecebda4f4a9b430_Screen-Shot-2020-11-.png)

To calculate the BLEU score you can do the following.

![](7uZFFyQ_QmamRRckP9Jmxw_2228df50ef0b4602b8721ea740ec5caa_Screen-Shot-2020-11-.png)

You would sum over the unique n-gram counts in the candidate and divide by the total number of words in the candidate. The same concept could apply to unigrams, bigrams, etc. One issue with the BLEU score is that it does not take into account semantics, so it does not take into account the order of the n-grams in the sentence.

Another similar method for evaluation is the ROUGE score which calculates precision and recall for machine texts by counting the n-gram overlap between the machine texts and a reference text.  Here is an example that calculates recall: 

![](BeSWnnMgQ3Wklp5zIKN1KA_0f153cafd62349dab83bd52de5698fb7_Screen-Shot-2020-11-.png)

Rouge also allows you to compute precision as follows: 

![](x7fvfymWSny3738plop8Eg_c1c4a60eb4af4e52916b27d82633a11d_Screen-Shot-2020-11-.png)
