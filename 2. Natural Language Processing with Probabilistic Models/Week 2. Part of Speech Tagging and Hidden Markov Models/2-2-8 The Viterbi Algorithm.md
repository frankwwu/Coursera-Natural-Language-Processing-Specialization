# The Viterbi Algorithm

The Viterbi algorithm makes use of the transition probabilities and the emission probabilities as follows. 

![](kG2A8zPoQu-tgPMz6ALvug_eab59a94f94c48f0bd3c82da894785b3_Screen-Shot-2021-03-10-at-2.48.55-PM.png)

To go from \piπ to ***O*** you need to multiply the corresponding transition probability (0.3) and the corresponding emission probability (0.5), which gives you 0.15. You keep doing that for all the words, until you get the probability of an entire sequence. 

![](UocLF3wnRiOHCxd8J4YjFw_a20bff55a54d4e649fc0b31c6177062c_Screen-Shot-2021-03-10-at-2.51.27-PM.png)

You can then see how you will just pick the sequence with the highest probability. We will show you a systematic way to accomplish this (Viterbi!). 
