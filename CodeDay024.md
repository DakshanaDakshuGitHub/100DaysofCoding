## Given a sequence of distinct non-negative integers, where each number is written in a separate line. The sequence ends with 0. Print the second largest element in this sequence. It is guaranteed that the sequence has at least two elements.
```
Example input
1
7
9
0

Example output
7
```
x = int(input())

arr=[]

while x!= 0:

arr.append(x)

x = int(input())

arr=[int(x) for x in arr]

arr.sort()

print(arr[-2])
