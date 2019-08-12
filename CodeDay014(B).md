## Write a program that receives a number on the input. - If the number is a multiple of 3, it prints "Jugs".  - If the number is a multiple of 5, it prints "Mugs". - If the number is a multiple of 7, it prints "Pugs". - If the number is a multiple of both 3 and 5, it prints "JugsMugs". - If the number is a multiple of both 3 and 7, it prints "JugsPugs". - If the number is a multiple of both 5 and 7, it prints "MugsPugs". - If the number is a multiple of both 3, 5 and 7, it prints "JugsMugsPugs".Otherwise, it prints the number. If the boolean 'rev' is True (or 1), then reverse the order of printing.   - "PugsJugsMugs" for multiples of 3, 5 and 7  - "PugsMugs" for multiple of 5 and 7  - "MugsJugs" for multiple of 3 and 5   - "PugsJugs" for multiple of 3 and 7
```
INPUT 
5
0
OUTPUT
1
2
Jugs
4
Mugs

INPUT 
15
1
OUTPUT
1
2
Jugs
4
Mugs
Jugs
Pugs
8
Jugs
Mugs
11
Jugs
Jugs
Pugs
MugsJugs
```
a=int(input())

rev=int(input())

for i in range(1,a+1):

if rev :

string= 'Jugs'* bool(i%3==0 or '3' in str(i))

string= 'Mugs'* bool(i%5==0 or '5' in str(i))+ string

string= "Pugs"* bool(i%7==0 or '7' in str(i))+ string

print(string or i)

else :

print("Jugs"* (i%3==0 or '3' in str(i)) + "Mugs"* (i%5==0 or '5' in str(i)) + "Pugs"* (i%7==0 or '7' in str(i)) or i)


    
   
 
