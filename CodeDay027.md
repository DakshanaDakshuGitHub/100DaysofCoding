## Given a list of numbers, find and print all its elements that are greater than their left neighbor.
```
Example input
1 5 2 4 3

Example output
5 4
```
a = [int(s) for s in input().split()]

for i in range(1,len(a)):
  
  if a[i] > a[i- 1]:
  
  print(a[i],end =' ')
