
Rank <= 6.5 means that every comedian with a rank of 6.5 or lower will follow the True arrow (to the left), and the rest will follow the False arrow (to the right).
gini = 0.497 refers to the quality of the split, and is always a number between 0.0 and 0.5, where 0.0 would mean all of the samples got the same result, and 0.5 would mean that the split is done exactly in the middle.
samples = 13 means that there are 13 comedians left at this point in the decision, which is all of them since this is the first step.

value = [6, 7] means that of these 13 comedians, 6 will get a "NO", and 7 will get a "GO".

Gini
There are many ways to split the samples, I have use the GINI method.
The Gini method uses this formula:
Gini = 1 - (x/n)2 - (y/n)2

Where x is the number of positive answers("GO"), n is the number of samples, and y is the number of negative answers ("NO"), which gives us this calculation:
1 - (7 / 13)2 - (6 / 13)2 = 0.497

True - 5 Comedians End Here:
gini = 0.0 means all of the samples got the same result.
samples = 5 means that there are 5 comedians left in this branch (5 comedian with a Rank of 6.5 or lower).
value = [5, 0] means that 5 will get a "NO" and 0 will get a "GO".

False - 8 Comedians Continue:
Nationality
Nationality <= 0.5 means that the comedians with a nationality value of less than 0.5 will follow the arrow to the left (which means everyone from the UK, ), and the rest will follow the arrow to the right.
gini = 0.219 means that about 22% of the samples would go in one direction.
samples = 8 means that there are 8 comedians left in this branch (8 comedian with a Rank higher than 6.5).
value = [1, 7] means that of these 8 comedians, 1 will get a "NO" and 7 will get a "GO".
