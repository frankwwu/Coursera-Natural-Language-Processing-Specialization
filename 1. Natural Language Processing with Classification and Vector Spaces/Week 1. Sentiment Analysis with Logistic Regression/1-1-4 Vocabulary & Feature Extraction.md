# Vocabulary & Feature Extraction

Given a tweet, or some text, you can represent it as a vector of dimension V, where V corresponds to your vocabulary size. If you had the tweet "I am happy because I am learning NLP", then you would put a 1 in the corresponding index for any word in the tweet, and a 0 otherwise. 

![](vpVZPKHCS6uVWTyhwmurrQ_d2e2fd874a354ab38047.png)

As you can see, as V gets larger, the vector becomes more sparse. Furthermore, we end up having many more features and end up training \theta V parameters. This could result in larger training time, and large prediction time. 