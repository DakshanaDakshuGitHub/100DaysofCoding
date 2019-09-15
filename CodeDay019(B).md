## The Missing Spy Plane!!The Indian Air Force (IAF)  is using more than 10,000 spy planes to  go across LoC to scout for terrorist camps in Pakistan. Whenever a spy   plane takes off for reconnaissance, the Plane ID is added to a list.  Whenever the plane returns, the ID is again added to the same list.   One spy plane alone has gone missing, so its ID was not added to the  list a second time.  By the way, IDs are not guaranteed to be  sorted or sequential.   1. Given a list of plane IDs, write a program to print out the ID of the missing spy plane. 2. If no plane is found missing, then print "All arrived!"  

```
INPUT
6
10001
10002
10003
10001
10003
10002

OUTPUT
All arrived!
```
a= int(input())

x=[]

d='All arrived'

for i in range(a):

n = int(input())

x.append(n)

for i in range(a):

c=x[i]

if x.count(c)% 2 != 0:

d=x[i]

print(d)
  
  
