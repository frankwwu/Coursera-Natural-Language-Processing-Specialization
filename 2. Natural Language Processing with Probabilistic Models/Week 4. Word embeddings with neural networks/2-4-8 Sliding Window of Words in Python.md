# Sliding Window of words in Python

![](5GCbimNSSeKgm4pjUlni1g_33285a93db5647628c0e62b82ed879ac_Screen-Shot-2021-03-29-at-10.41.52-AM.png)

The code above shows you a function which takes in two parameters. 

* Words: a list of words.
* C: the context size.

We first start by setting *i* to C. Then we single out the center_word, and the context_words. We then yield those and increment *i*. 