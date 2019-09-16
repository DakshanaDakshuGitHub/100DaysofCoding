## Write a program to calculate the distance between two points.
#### SAMPLE:
```
Example 

INPUT 
4
0
0
0

OUTPUT
4
```
#### PROGRAM:
```
x1 = int(input())  
y1 = int(input())  
x2 = int(input())
y2 = int(input())
distance = (((x2 - x1) ** 2) + ((y2 - y1) ** 2)) ** 0.5 
print(distance)
```
