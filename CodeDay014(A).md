## Write a program that receives a number on the input. - If the number is a multiple of 3, it prints "Jugs".  - If the number is a multiple of 5, it prints "Mugs". - If the number is a multiple of 7, it prints "Pugs". - If the number is a multiple of both 3 and 5, it prints "JugsMugs". - If the number is a multiple of both 3 and 7, it prints "JugsPugs". - If the number is a multiple of both 5 and 7, it prints "MugsPugs". - If the number is a multiple of both 3, 5 and 7, it prints "JugsMugsPugs".Otherwise, it prints the number. If the boolean 'rev' is True (or 1), then reverse the order of printing.   - "PugsJugsMugs" for multiples of 3, 5 and 7  - "PugsMugs" for multiple of 5 and 7  - "MugsJugs" for multiple of 3 and 5   - "PugsJugs" for multiple of 3 and 7

```
INPUT 
73 
False  # contains 3 and 7

OUTPUT
JugsPugs

INPUT 
73 
True  # contains 7 and 3, print reverse order

OUTPUT
PugsJugs

INPUT 
51  # multiple of 3 and contains 5

OUTPUT
JugsMugs


INPUT 
105

OUTPUT 
JugsMugsPugs

```
i=int(input())

rev=int(input())

if rev :

string= 'Jugs'* bool(i%3==0 or '3' in str(i))

string= 'Mugs'* bool(i%5==0 or '5' in str(i))+ string

string= "Pugs"* bool(i%7==0 or '7' in str(i))+ string

print(string or i)

else :

print("Jugs"* (i%3==0 or '3' in str(i)) + "Mugs"* (i%5==0 or '5' in str(i)) + "Pugs"* (i%7==0 or '7' in str(i)) or i)


    
