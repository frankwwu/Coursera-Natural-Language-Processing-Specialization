# Naive Bayes Introduction

To build a classifier, we will first start by creating conditional probabilities given the following table:

![](fwihrJk_RSGIoayZPxUhTQ_3cd35492d526492dbcae2e4baa02.png)

This allows us compute the following table of probabilities:

![](Iiek1X0pSX6npNV9KXl-NQ_2945fa3844184948b0a2590d0683.png)

Once you have the probabilities, you can compute the likelihood score as follows

![](nc3XUyPHSgyN11Mjx7oMNQ_d2a00c93d29b497bba81a3944072.png)

A score greater than 1 indicates that the class is positive, otherwise it is negative.