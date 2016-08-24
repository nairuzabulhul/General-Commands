
### Use split(), for loop and if statement to solve this problem 
### return only words that start with letter 's'

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
