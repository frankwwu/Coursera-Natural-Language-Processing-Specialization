# Minimum edit distance algorithm II

To populate the following table: 

![](O-f54Zf1QfCn-eGX9aHwBg_44c4b8325c0841cda5db5635ebb50217_Screen-Shot-2021-03-01-at-3.26.04-PM.png)

There are three equations: 

* **D[i,j] = D[i-1, j] + del_cost**: this indicates you want to populate the current cell (i,j) by using the cost in the cell found directly above. 
* **D[i,j] = D[i, j-1] + ins_cost**: this indicates you want to populate the current cell (i,j) by using the cost in the cell found directly to its left. 
* **D[i,j] = D[i-1, j-1] + rep_cost**: the rep cost can be 2 or 0 depending if you are going to actually replace it or not. 

At every time step you check the three possible paths where you can come from and you select the least expensive one. Once you are done, you get the following: 

![](6fFcxaBxQrSxXMWgcZK0QA_02ee3706678a4cb383f5e972bd1879f9_Screen-Shot-2021-03-01-at-3.36.05-PM.png)

