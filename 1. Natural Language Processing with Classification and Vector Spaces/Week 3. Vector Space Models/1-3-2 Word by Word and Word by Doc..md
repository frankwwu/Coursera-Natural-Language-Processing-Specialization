# Word by Word and Word by Doc.

<u>**Word by Word Design**</u>

We will start by exploring the word by word design. Assume that you are trying to come up with a vector that will represent a certain word.  One possible design would be to create a matrix where each row and column corresponds to a word in your vocabulary. Then you can iterate over a document and see the number of times each word shows up next each other word. You can keep track of the number in the matrix. In the video I spoke about a parameter KK. You can think of KK as the bandwidth that decides whether two words are next to each other or not. 

![](Bl9oAms0R4yfaAJrNJeMMQ_d1093d07494248b6bcfd656363fba2d9_Screen-Shot.png)

In the example above, you can see how we are keeping track of the number of times words occur together within a certain distance kk. At the end, you can represent the word data, as a vector v = [2,1,1,0]v=[2,1,1,0].

<u>**Word by Document Design**</u>

You can now apply the same concept and map words to documents. The rows could correspond to words and the columns to documents. The numbers in the matrix correspond to the number of times each word showed up in the document. 

![](XXPXAWtOTAqz1wFrTqwK6w_741e4935c5ac435a96373dd745b124f9_Screen-Shot.png)

You can represent the entertainment category, as a vector v = [500, 7000]v=[500,7000]. You can then also compare categories as follows by doing a simple plot. 

![](IkrSkusORvCK0pLrDpbwRQ_3ab7a81281fb491dbd0736f83b095b2a_Screen-Shot.png)

Later this week, you will see how you can use the angle between two vectors to measure similarity. 