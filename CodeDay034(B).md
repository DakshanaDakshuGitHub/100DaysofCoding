### You are given a dictionary consisting of word pairs. Every word is a synonym of the other word in its pair. All the words in the dictionary are different.After the dictionary there's one more word given. Find a synonym for it.
#### SAMPLE:
```
Example input
3
Hello Hi
Bye Goodbye
List Array
Goodbye

Example output
Bye
```
#### PROGRAM:
```
# Read a string:
# Print a value:
# print(s)
n = int(input())
dic = {}
s = list(input().split())
for i in range (n):
    dic[s[0]] = s[1]
    if i < n-1:
        s = list(input().split())
word = input()
for k, v in dic.items():
    if k == word:
        print(v)
    if v == word:
        print(k)
```
