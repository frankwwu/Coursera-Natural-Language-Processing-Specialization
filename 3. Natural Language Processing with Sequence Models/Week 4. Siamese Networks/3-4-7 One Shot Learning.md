# One Shot Learning

Imagine you are working in a bank and you need to verify the signature of a check. You can either build a classifier with K possible signatures as an output or you can build a classifier that tells you whether two signatures are the same. 

![](-c1tDMazR5SNbQzGs0eU3Q_7011ed8e6ee2401f875d32827922964d_Screen-Shot-2021-04-13-at-3.29..png)

Hence, we resort to one shot learning. Instead of retraining your model for every signature, you can just learn a similarity score as follows: 

![](5rDS_cszTvew0v3LM5737A_e41f8b11711c41ca984bc6c0524b31ae_Screen-Shot-2021-04-13-at-3.31..png)