## Conditions and Branching
- comparison operator
- 'a'=='A' will return False
- Branching using if else
- equal: ==
- not equal: !=
- greater than: >
- less than: <
- greater than or equal to: >=
- less than or equal to: <=

```
# Elif statment example

age = 18

if age > 18:
    print("you can enter" )
elif age == 18:
    print("go see Pink Floyd")
else:
    print("go see Meat Loaf" )
    
print("move on")
```

```
if(condition):
  do some task
elif(condition):
  do some task
else:
  do some task
```
- logical operators.... operates on boolean
- or, and (condition) or (condition) ~~ return true if either condition is true else false
- ASCII (A-Z ~~ 65-90 a-z ~~ 97-122)

- LOGICAL OPERATORS: and or not

## Loops
- range(N) return ordered sequuence from 1 to N-1
- The range() function returns a list or sequence of numbers
- for(i in range(3)):
- for square in squares:   ~~ iterates through the squares list and stores each element in square variable everytime
- enumerate in python returs the element and index
```
for i, square in enumerate(squares):
    print(i, square)
```
```
count = 1
while count <= 5:
    print(count)
    count += 1
```
## Functions
- a piece of code that can be reused.. takes an input and returns output
- built-in function
- len()  takes the input of the type sequence
- sorted() results sorted list [doesn't changes the original list]
- A.sort() sorts and changes the original list itself
```
def add1(a):
 b=a+1
 return b

add1(5)

OUTPUT: 6
```
- a function can have multiple parameters
- if the function doesn't return nothing, python returns the special none object
- pass keyword doesn't do anything... can be used in a function body to pass python being non empty function body
- variadic parameters helps to store value with error of number of parameter
- global scope and local scope
- keyword Global use to declare global variable
-   
- 
- 
















 
