## Given a three-digit number. Find the sum of its digits.
```
Example input
123

Example output
6
```
num = int(input())

sum = 0

while(num != 0):

n = num % 10

sum = sum + n

num = num // 10

print(sum)
