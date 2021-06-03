# Computing the Cost I

To compute the cost, we will prepare the batches as follows: 

![](_5Dt7pRoT5aQ7e6UaJ-Wtg_3626f14327644dc3b3b129c97389d4e4_Screen-Shot-2021-04-13-at-2.42..png)

Note that each example, has a similar example to its right, but no other example means the same thing. We will now introduce hard negative mining. 

![](sKKWDGkoTt6ilgxpKP7eiw_d3433c4628544c0a8d1b8da5b70b42b6_Screen-Shot-2021-04-13-at-2.49..png)

Each horizontal vector corresponds to the encoding of the corresponding question. Now when you multiply the two matrices and compute the cosine, you get the following: 

![](y5_oPy-KRTyf6D8viuU8Eg_ff3c1f8337484d1c8c246aabc88587bf_Screen-Shot-2021-04-13-at-3.00..png)

The diagonal line corresponds to scores of similar sentences, (normally they should be positive). The off-diagonals correspond to cosine scores between the anchor and the negative examples. 