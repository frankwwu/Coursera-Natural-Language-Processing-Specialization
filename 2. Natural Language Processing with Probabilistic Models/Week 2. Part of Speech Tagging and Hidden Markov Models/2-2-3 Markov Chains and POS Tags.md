# Markov Chains and POS Tags

To help identify the parts of speech for every word, you need to build a transition matrix that gives you the probabilities from one state to another.  

![](90NgMEU-R4GDYDBFPmeB1w_200e80a6b784467e872d8bfa22fb3ac8_Screen-Shot-2021-03-10-at-12.07.50-PM.png)

In the diagram above, the blue circles correspond to the part of speech tags, and the arrows correspond to the transition probabilities from one part of speech to another. You can populate the table on the right from the diagram on the left. The first row in your **A** matrix corresponds to the initial distribution among all the states. According to the table, the sentence has a 40% chance to start as a noun, 10% chance to start with a verb, and a 50% chance to start with another part of speech tag. 

In more general notation, you can write the transition matrix **A**, given some states **Q**, as follows: 

![](KBo6VZmGT9KaOlWZhg_SaQ_b77c6dd0a92a496d94f6ad72d507a827_Screen-Shot-2021-03-10-at-12.15.50-PM.png)
