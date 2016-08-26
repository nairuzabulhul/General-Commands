# Problem 1:

#### Use split(), for loop and if statement to solve this problem 
#### return only words that start with letter 's'

str = "Print only the words that start with s in this sentence"

```
#Method 1:

strSplit = str.split()
emp_list = []

# if the index of the letter == s return the word
for letter in strSplit :
    if letter[0] == 's':
        emp_list.append(letter)

print emp_list        
```           

```
# Method 2:            
# List Comprehension:

# print [letter for letter in strSplit if letter[0] == 's']

```

#Problem 2

#### Use range() to print all even numbers from (0 , 10)
```
#Method 1:
num_list = []

for x in range(0,10):
    if x % 2 == 0 :
        num_list.append(x)

print num_list
```
```
#Method 2:
# Using List Comprehension

print [ num for num in range(0,10) if num % 2 == 0 ]
```


# Problem 3:

```
# Use List comprehension to create a list of all numbers between 
# 1 and 50 that are divisible by 3

print [num for num in range(1,50) if num % 3 == 0 ]

```

# Problem 4:

```
## Go through the string below and if the length of a word is even print "even"
# "Print every word in this sentence that has an even nymber of letters"

str = "Print every word in this sentence that has an even number of letters"

strSplit = str.split()

print strSplit


for x in strSplit:
    if len(x) % 2 == 0:
        print "even"
```

# Problem 5:

```
""" Write a program that prints that integers from 1 to 100. But for mulitple of three print "Fizz" instead of the number
    , and for the multiples of five print "Buzz".
    For numbers which aree multiples of both
    three and five print "FizzBuzz"
"""

num = []

for x in range(1,100):
    if x % 3 == 0:
        num.append("Fizz")
    elif x % 5 == 0 :
        num.append("Buzz")
    
    elif x % 3 == 0  and x % 5  == 0 :
        num.append("FizzBuzz")
        

print num
```

# Problem 6 :

