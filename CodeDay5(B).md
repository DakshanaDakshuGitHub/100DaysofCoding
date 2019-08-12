## Given the integer N - the number of seconds that is passed since midnight - how many full hours and full minutes are passed since midnight?
```
Example input
3900

Example output
1 65
```
sec = int(input())

hr = sec // 3600

min = sec // 60 

print(hr, min)
