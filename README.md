LAB03 EXERCISES

Find All Duplicates
Write a function (or static method in the case of Java) that accepts a list of integers
and returns a list of only those integers that appear more than once.

Describe Different Approaches to Solving This Problem
Describe the two different ways to figure out all of the duplicate values of a list of 
integers in english. The first solution is the nested loop solution. The second solution 
is to use a dictionary or a map (similar to the containsPair method we wrote in 
class. Describe both in as much detail as you can (with no code) and describe the
trade-offs between the two solutions.

The first method is to use a nested for loop in another for loop. The first
for loop starts from the first value in the list and loops through the whole
list. The nested for loop starts from the 2nd value and loops through the
whole list. This way, every value is compared to each other. Inside of the
nested for loop, there is an if statement to compare the values and check 
if the duplicate value is already in the list. If it isn't, then it's added to the list.

The second method uses a dictonary or a hash map to efficiently keep track
of values we have already seen before. As it iterates through the list, the
dictionary keeps the count of each element. At the end, we can go through 
the dictionary and take all the values that are greater than 1 to get the duplicates.

The trade offs have to do with the efficiency and simplicity. The efficiency 
of the first method is of O(n^2) and for the second method it's just O(n).
The second method is more efficient and would be faster with larger datasets. On the other hand, the first method is simpler and easier to understand. 
