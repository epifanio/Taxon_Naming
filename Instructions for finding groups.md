# Instructions for finding groups of similar names

1. Take the whole list of names ("Names", of length n), and grab the first name on it. Put it in an object "Group 1"
2. Calculate the similarity between this name (Names[1]) and all the other names (Names[2,...n]). Save in a data frame (or list? "Result") with two columns, each Names[2,...n], and the similarity value obtained
3. Find in "Result" all rows where the value in the second column is greater than a threshold T (typically a value close to 100, e.g. 90)
4. Grab the corresponding names. Total number, r
5 Add the r names to "Group 1". The length of "Group 1" is now r + 1
6. Remove the same r names from Names
7. The new Names is now n - r - 1
8. Repeat from 1 until no more items remain in Names
