### The text is given in a single line. For each word of the text count the number of its occurrences before it.
#### SAMPLE:
```
Example input
one two one two three two four three

Example output
0 0 1 1 0 2 0 1
```
#### PROGRAM:
```
# Read a string:
a = input().split()
b={}
# Print a value:
# print(s)
for i in a:
  if i not in b:
    b[i]=0
  print(b[i],end='')
  b[i] += 1
  ```
