# Logistic Regression: Testing

To test your model, you would run a subset of your data, known as the validation set, on your model to get predictions. The predictions are the outputs of the sigmoid function. If the output is \geq=0.5, you would assign it to a positive class. Otherwise, you would assign it to a negative class. 

![](xq8RYoHvROKvEWKB73TiUg_ac2e78d0c6654f58ab40.png)

In the video, I briefly mentioned X validation. In reality, given your XX data you would usually split it into three components. X_{train}, X_{val}, X_{test}. The distribution usually varies depending on the size of your data set. However, an 80, 10, 10 split usually works fine. 

To compute accuracy, you solve the following equation: 

![](1NW_9EVkS6yVv_RFZGusFA_90304c432911444eb5f9.png)

In other words, you go over all your training examples, mm of them, and then for every prediction, if it was wright you add a one. You then divide by mm. 

