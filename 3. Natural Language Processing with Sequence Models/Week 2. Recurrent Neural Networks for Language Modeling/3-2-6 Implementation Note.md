# Implementation Note

The scan function is built as follows: 

![](V-DXCJC8SZ6g1wiQvCmeOg_611f063635804b99b4a5226478045857_.png)

Note, that is basically what an RNN is doing. It takes the initializer, and returns a list of outputs (ys), and uses the current value, to get the next y and the next current value. These type of abstractions allow for much faster computation. 