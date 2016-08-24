## List Comprehension 
```
# general rule:

[ output for item in list ]

- output you want to get from the for loop
- item is the items inside the list 
- list is the array or list itself

```

1- Pushing items to the list 

```
l = []

for x in "word" :
  l.append(x)
```

### Output:
  l = ['w','o','r',d]


## Using list Comprehension 

```
l = [ x for x in 'word']
```

### Output:
  l = ['w','o','r',d]

  
## List Comprehension using for loop and if statement

```
newList = [ x for x in range(5) if x %2 == 0 ]
```
### Output should ONLY return a list with numbers that are divisible by 2 
newList = [0, 2, 4]

```
celsius = [0, 10, 20.6]
newList = [ (temp * (9/5.0) +32) for temp in  celsius ]
```
### Output returns a list with frehenheit temps
newList = [32.0 , .............. ]


# Nested List Comprehesion :
```
x = [0, 10, 20.6]
newList = [ x ** 2 for x in  [ x ** 2 for x in range(11)] ]
```
### Output returns a list with numbers to fourth power
newList = [...,....,....]








  
  


