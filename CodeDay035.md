### The first line contains the number of records. After that, each entry contains the name of the candidate and the number of votes they got in some state. Count the results of the elections: sum the number of votes for each candidate. Print candidates in the alphabetical order.
#### SAMPLE:
```
Example input
5
McCain 10
McCain 5
Obama 9
Obama 8
McCain 1

Example output
McCain 16
Obama 17
```
#### PROGRAM:
```
n = {} 
for _ in range(int(input())):
  a,v=input().split()
  n[a]=n.get(a,0)+ int(v)
for a,v in sorted(n.items()):
  print(a,v)
 ```
