### Given the year number. You need to check if this year is a leap year. If it is, print LEAP, otherwise print COMMON.
#### SAMPLE:
```
Example input
2012

Example output
LEAP
```
#### PROGRAM:
```
a = int(input())
if a % 4 == 0 and a % 100 != 0 :
   print("LEAP")
elif a % 400 == 0 :  
   print("LEAP")
else:
   print("COMMON")
```
