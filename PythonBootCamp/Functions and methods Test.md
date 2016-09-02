# Problem 1:

Write a function that computes the volume of a sphere given its radius.

```
import math

"""
# Sphere Volume:
V = 4/3 pi * r ** 3
"""

def vol(rad):
    
    volume = float(((math.pi * 4)* rad**3) /3)
    
    return volume
    
print vol(5)
```

# Problem 2:

Write a function that checks whether a number is in a given range (inclusive of high and low)
1- return a print statement
2- return a Boolean

```
# Method 1 : return a print statement 
def ran_check(num, low, high):
    
    number_range = range(low, high) #use range
    
    if num in number_range:
        print num , "is in the range"
    
    else:
        print num , "is NOT in the range"
        
print ran_check(30, 0, 10) 
print ran_check(3, 0, 10) 
```

```
# Method 2: return a Boolean
def ran_bool(num, low, high):
    
    number_range = range(low, high)
    
    if num in number_range:
        return True
    
    else:
        return False
        
print ran_bool(30, 0, 10) #returns False
print ran_bool(3, 0, 10) #returns True
```


# Problem 3:

Write a function that accepts a string and calculate the number of uppercase letters and lower case letters
Sample String:
'Hello Mr. Rogers, how are you this fine Tuesday?'

```
def count_letters(str):
    uppercase_letters = 0
    lowercase_letters = 0
    
    for letters in str:
        
        if letters.isupper():
            uppercase_letters +=1
        
        if letters.islower():
           lowercase_letters += 1
        
    print "Upper case letters: ", uppercase_letters , "Lower case letters", lowercase_letters  

print count_letters("Hello Mr. Rogers, how are you this fine Tuesday?")

#Strategy :
1- Create a counter for lowercase letters and uppercase letters
2- For loop through the string and use isupper()/ islower() to check the letter
3- print the numbers of upper letters and lower letters
```

# Problem 4:

Write a function that takes a list and returns a new list with unique elements from the first list 
```
def unique_list(l):

    result = set(l)
    
    return list(result)

num_list = [1,1,1,2,7,5,5,3,3]

print unique_list(num_list)

# Strategy :
1- use set function, it removes duplicates in the list
2- cast set as list to return a list of unique numbers
```

# Problem 5 :

Write a function to multiply all the numbers in a list
```
def multi_list(l):

    sum_of_number = 0 
    
    for num in l :
        sum_of_number += num
    
    return sum_of_number

num_list = [1,2,3,2]
print multi_list(num_list)

#Strategy:
1- create a counter to add the numbers to
2- for loop through the list and add every elements to the "sum_of_number"
3- return the sum_of_number
```

# Problem 6:

