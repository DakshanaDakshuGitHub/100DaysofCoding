## For given integer n ≤ 9 print a ladder of n steps. The k-th step consists of the integers from 1 to k without spaces between them.To do that, you can use the sep and end arguments for the function print().

```
Example input
3

Example output
1
12
123
```
a = int(input())

for row in range(1,a+1):

for column in range(1,row+1):

print(column, end="")

print("")
