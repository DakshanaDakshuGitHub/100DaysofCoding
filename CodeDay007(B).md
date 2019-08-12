## Given three integers, print the least of them.
```
Example input
5
3
7

Example output
3
```
a = int(input())

b = int(input())

c = int(input())

if(c < a):
 
    if(c < b):
 
    print(c)

elif(b < a):
 
    print(b)

else:

    print(a)
