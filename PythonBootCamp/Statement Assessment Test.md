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
