# Computing Accuracy

To compare the accuracy, just follow the following steps:

* Pass test set through the model 
* Get arg max across the prediction array
* Mask padded tokens
* Compare with the true labels. 