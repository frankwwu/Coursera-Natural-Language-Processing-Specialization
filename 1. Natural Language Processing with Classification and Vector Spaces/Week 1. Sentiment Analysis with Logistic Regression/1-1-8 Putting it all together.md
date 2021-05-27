# Putting it all together

Over all , you start with a given text, you perform preprocessing, then you do feature extraction to convert text into numerical representation as follows:

![](_OTVrbipS9ek1a24qXvXFw_641fc5c72d974a4582c2.png)

Your X becomes of dimension (m,3)(m,3) as follows.

![](C3BC-AlDRj-wQvgJQyY_8w_6b189b0ef72e456b9cce.png)

When implementing it with code, it becomes as follows:

![](NwmjyOjKQTaJo8joyqE2Ow_330a68fd246c44c3a540.png)

You can see in the last step you are storing the extracted features as rows in your XX matrix and you have mm of these examples. 