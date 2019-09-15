## For the given integer N calculate the following sum: 1³ + 2³ + ... + N³

```
Example input
3

Example output
36
```
a = int(input())

n=0

for i in range(1,a+1):

n+=i*i*i

print(n)
