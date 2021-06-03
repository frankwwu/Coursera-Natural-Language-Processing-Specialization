# Fine tuning BERT

Once you have a pre-trained model, you can fine tune it on different tasks. 

![](JAmRdPOJSBWJkXTziRgVVA_369ff270b1884dbca684aa3bed272976_Screen-Shot-2021-01-22-at-1..png)

For example, given a hypothesis, you can identify the premise. Given a question, you can find the answer. You can also use it for named entity recognition. Here is a summary of the inputs.

![](PFTBnd1DQXSUwZ3dQzF0jg_e8a9f7039ada47ccbdd395a422de024c_Screen-Shot-2021-01-22-at-1..png)

* You can replace sentences A/B
* Paraphrase from sentence A
* Question/passage
* Hypothesis premise pairs in entailment
* Text and a Ø for classification/sequence tagging
* Output tokens are fed into a layer for token level tasks otherwise use [CLS] embedding as input.
 