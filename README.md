## Question1.-> A bracket is considered to be any one of the following characters: (, ), {, }, [, or ].
Two brackets are considered to be a matched pair if the opening bracket (i.e., (, [, or {) occurs to the left of a closing bracket (i.e., ), ], or }) of the exact same type. There are three types of matched pairs of brackets: [], {}, and ().
A matching pair of brackets is not balanced if the set of brackets it encloses are not matched. For example, {[(])} is not balanced because the contents in between { and } are not balanced. The pair of square brackets encloses a single, unbalanced opening bracket, (, and the pair of parentheses encloses a single, unbalanced closing square bracket, ].
By this logic, we say a sequence of brackets is balanced if the following conditions are met:
It contains no unmatched brackets.
The subset of brackets enclosed within the confines of a matched pair of brackets is also a matched pair of brackets.
Given  strings of brackets, determine whether each sequence of brackets is balanced. If a string is balanced, return YES. Otherwise, return NO.
Function Description
Complete the function isBalanced in the editor below.
isBalanced has the following parameter(s):
string s: a string of brackets
Returns
string: either YES or NO
Input Format
The first line contains a single integer , the number of strings.
Each of the next  lines contains a single string , a sequence of brackets
, where  is the length of the sequence.
All characters in the sequences ∈ { {, }, (, ), [, ] }.
Output Format
For each string, return YES or NO.

`Sample Input`
```js
STDIN           Function
-----           --------
3               n = 3
{[()]}          first s = '{[()]}'
{[(])}          second s = '{[(])}'
{{[[(())]]}}    third s ='{{[[(())]]}}'
```
`Sample Output`
```
YES
NO
YES
```
Explanation
The string {[()]} meets both criteria for being a balanced string.
The string {[(])} is not balanced because the brackets enclosed by the matched pair { and } are not balanced: [(]).
The string {{[[(())]]}} meets both criteria for being a balanced string.































## Question 2.-> Given a matrix of size r*c. Traverse the matrix in spiral form.
Example 1:
`Input:`
```
r = 4, c = 4
matrix[][] = {{1, 2, 3, 4},
           {5, 6, 7, 8},
           {9, 10, 11, 12},
           {13, 14, 15,16}}
```           
`Output:` 
```
1 2 3 4 8 12 16 15 14 13 9 5 6 7 11 10
```
![original1](https://user-images.githubusercontent.com/97151477/162397521-0ac0aa7e-acd4-4510-9b62-f40755df042f.png)


Example 2:
`Input:`
```
r = 3, c = 4  
matrix[][] = {{1, 2, 3, 4},
           {5, 6, 7, 8},
           {9, 10, 11, 12}}
```           
`Output:`
```
1 2 3 4 8 12 11 10 9 5 6 7
```
`Explanation:`
Applying same technique as shown above, 
output for the 2nd test case will be 
1 2 3 4 8 12 11 10 9 5 6 7.

 
`Your Task:`
```
You don't need to read input or print anything. Complete the function spirallyTraverse() that takes matrix, r and c as input parameters and returns a list of integers denoting the spiral traversal of matrix. 
Question 3.-> You are given a number N. Find the total count of set bits for all numbers from 1 to N(both inclusive).
```


## Question 3.-> You are given a number N. Find the total count of set bits for all numbers from 1 to N(both inclusive).
 
Example 1:
`Input:` N = 4
```
`Output:` 5
```
`Explanation:`
```
For numbers from 1 to 4.
For 1: 0 0 1 = 1 set bits
For 2: 0 1 0 = 1 set bits
For 3: 0 1 1 = 2 set bits
For 4: 1 0 0 = 1 set bits
Therefore, the total set bits is 5.
 
Example 2:
`Input:` N = 17
```
`Output:` 35
```
`Explanation:`
```
From numbers 1 to 17(both inclusive), 
The total number of set bits is 35.
 
`Your Task:` 
```
The task is to complete the function countSetBits() that takes n as a parameter and returns the count of all bits.
```
 
 
 
 
 
 
## Question 4.-> Given an array A of n positive numbers. The task is to find the first Equilibrium Point in the array. 
Equilibrium Point in an array is a position such that the sum of elements before it is equal to the sum of elements after it.
Note: Return the index of Equilibrium point. (1-based index)
`Example 1:`
`Input:`
``` 
n = 5 
A[] = {1,3,5,2,2} 
Output: 3 
```
`Explanation:`
```
For second test case 
equilibrium point is at position 3 
as elements before it (1+3) = 
elements after it (2+2). 
 
 
`Example 2:`
`Input:`
n = 1
A[] = {1}
Output: 1
Explanation:
Since its the only element hence
it's the only equilibrium point.
 
`Your Task:`
The task is to complete the function equilibriumPoint() which takes the array and n as input parameters and returns the point of equilibrium. Return -1 if no such point exists.


