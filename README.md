# MITx-6.00.1x
Problem Set 1 


problem set 1 
Solution: 

counter = 0

for i in s:
    if i == 'a' or i == 'e' or i == 'i' or i == 'o' or i == 'u':
        counter += 1

print('Number of vowels:', counter)


Problem Set 2
Assume s is a string of lower case characters.

Write a program that prints the number of times the string 'bob' occurs in s. For example, if s = 'azcbobobegghakl', then your program should print

Solution: 

counter = 0
for i in range(len(s) - 2):
    if s[i] == 'b' and s[i + 1] == 'o' and s[i + 2] == 'b':
        counter += 1

print ('Number of times bob occurs is:', counter)


Problem 3
Assume s is a string of lower case characters.

Write a program that prints the longest substring of s in which the letters occur in alphabetical order. For example, if s = 'azcbobobegghakl', then your program should print


Solution: 


count = 0
maxcount = 0
result = 0

for char in range(len(s) - 1):
    if (s[char] <= s[char + 1]):
        count += 1
        if count > maxcount:
            maxcount = count
            result = char + 1
    else:
        count = 0
startposition = result - maxcount
print('Longest substring in alphabetical order is:', s[startposition:result + 1])


