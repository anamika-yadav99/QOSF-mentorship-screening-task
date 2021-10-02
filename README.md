# QOSF-mentorship-screening-task
# Task 1 

Design a quantum circuit that considers as input the following vector of integers numbers: 

[1,5,7,10]  returns a quantum state which is a superposition of indices of the target solution, obtaining in the output the indices of the inputs where two adjacent bits will always have different values. In this case the output should be: 1/sqrt(2) * (|01> + |11>) , as the correct indices are 1 and 3.

1 = 0001

5 = 0101

7 = 0111

10 = 1010

The method to follow for this task is to start from an array of integers as input, pass them to a binary representation and you need to find those integers whose binary representation is such that two adjacent bits are different. Once you have found those integers, you must output a superposition of states where each state is a binary representation of the indices of those integers.

Example 1
Consider the vector [1,5,4,2]
Pass the integer values to binary numbers that is [001,101,100,010]
 Identifies which values whose binary representation is such that two adjacent bits are different, we can see that are 2 101 and 010, [001,101,100,010].
Returns the linear combination of the indices in which the values satisfying the criterion are found.
Indices:

   0     1      2  	3
   
   |       |      |      |
   
 [001,101,100,010]

Indices are converted to binary states

|00> |01> |10> |11>

|         |	      | 	 |

[001,101,100,010]

 The answer would be the superposition of the states |01> and |11> or 1/sqrt(2) * (|01> + |11>)
