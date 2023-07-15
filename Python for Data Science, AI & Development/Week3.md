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
- if the function doesn't return anything, python returns the special none object
- pass keyword doesn't do anything... can be used in a function body to pass Python being a non-empty function body
- variadic parameters help to store value with the error of the number of parameters
- global scope and local scope
- keyword Global use to declare a global variable
- count() return the count of the element in the list
```
# Python Program to Count words in a String using Dictionary
def freq(string):
    
    #step1: A list variable is declared and initialized to an empty list.
    words = []
    
    #step2: Break the string into list of words
    words = string.split() # or string.lower().split()
    
    #step3: Declare a dictionary
    Dict = {}
    
    #step4: Use for loop to iterate words and values to the dictionary
    for key in words:
        Dict[key] = words.count(key)
        
    #step5: Print the dictionary
    print("The Frequency of words is:",Dict)
    
#step6: Call function and pass string in it
freq("Mary had a little lamb Little lamb, little lamb Mary had a little lamb.Its fleece was white as snow And everywhere that Mary went Mary went, Mary went \
Everywhere that Mary went The lamb was sure to go")
``` 
- formal parameter also called argument
- default argument     (empty argument and default parameter)
- del myFavouriteBand ~~ deletes a variable
- When the number of arguments are unknown for a function, They can all be packed into a tuple as shown:
```
def printAll(*args): # All the arguments are 'packed' into args which can be treated like a tuple
    print("No of arguments:", len(args)) 
    for argument in args:
        print(argument)
#printAll with 3 arguments
printAll('Horsefeather','Adonis','Bone')
#printAll with 4 arguments
printAll('Sidecar','Long Island','Mudslide','Carriage')

-----

def printDictionary(**args):
    for key in args:
        print(key + " : " + args[key])

printDictionary(Country='Canada',Province='Ontario',City='Toronto')

def addItems(list):
    list.append("Three")
    list.append("Four")
​
myList = ["One","Two"]
​
addItems(myList)
​
myList
    
['One', 'Two', 'Three', 'Four']



------

# Python Program to Count words in a String using Dictionary
def freq(string,passedkey):

    #step1: A list variable is declared and initialized to an empty list.
    words = []

    #step2: Break the string into list of words
    words = string.split() # or string.lower().split()

    #step3: Declare a dictionary
    Dict = {}

    #step4: Use for loop to iterate words and values to the dictionary
    for key in words:
        if(key == passedkey):
            Dict[key] = words.count(key)   
    #step5: Print the dictionary
    print("Total Count:",Dict)

#step6: Call function and pass string in it
freq("Mary had a little lamb Little lamb, little lamb Mary had a little lamb.Its fleece was white as snow And everywhere that Mary went Mary went, Mary went \
Everywhere that Mary went The lamb was sure to go","little")

```


## Exception Handling
- exceptional handling helps to run the program without termination in case of error.
- try and except , else and finally block
```
try:
    print(1+'ada')
except: 
    print('some error occurred)
finally:
    print("code run successfully")

--
some error occurred
code run succesfulluy
```
- ZeroDivisionError occurs when you try to divide by zero. 1/0
- NameError -- in this case, it means that you tried to use the variable a when it was not defined.
- IndexError -- in this case, it occured because you tried to access data from a list using an index that does not exist for this list.
- https://docs.python.org/3/library/exceptions.html
- int(input("enter a number"))
```
try:
    # code to try to execute
except(ZeroDivisionError, NameError):
    # code to execute if there is an exception of the given types
    
# code that will execute if there is no exception or a one that we are handling

---
# potential code before try catch

try:
    # code to try to execute
except ZeroDivisionError:
    # code to execute if there is a ZeroDivisionError
except NameError:
    # code to execute if there is a NameError
    
# code that will execute if there is no exception or a one that we are handling
---

a = 1

try:
    b = int(input("Please enter a number to divide a"))
    a = a/b
    print("Success a=",a)
except ZeroDivisionError:
    print("The number you provided cant divide 1 because it is 0")
except ValueError:
    print("You did not provide a number")
except:
    print("Something went wrong")

## Output : You did not provide a number        
------
# potential code before try catch

try:
    # code to try to execute
except ZeroDivisionError:
    # code to execute if there is a ZeroDivisionError
except NameError:
    # code to execute if there is a NameError
except:
    # code to execute if ther is any exception
else:
    # code to execute if there is no exception
finally:
    # code to execute at the end of the try except no matter what
    
# code that will execute if there is no exception or a one that we are handling

---


a = 1

try:
    b = int(input("Please enter a number to divide a"))
    a = a/b
except ZeroDivisionError:
    print("The number you provided cant divide 1 because it is 0")
except ValueError:
    print("You did not provide a number")
except:
    print("Something went wrong")
else:
    print("success a=",a)
finally:
    print("Processing Complete")

```

## Objects and Classes
- int, float, string, list, dictionary, boolean
- every object has type, internal rep, set of methods to onteract
- object is an instance of a particular type
- A.reverse() ~~ A is a list
- Crete own type or class
- class contains data attribute and methods
```
class Circle(object):
#class def     class parent

  def __init__(self, radius, color):   ##init: constructor. That tells python, we are creating a class(self is the newly created instance and rest and attributes)
    self.radius=radius;
    self.color=color;

  def add_radius(self,r):
    self.radius=self.radius+r

RedCircle = Circle(10,"red") ~~ object creation
RedCircle.radius ## return 10
RedCircle.radius=20 ## changes the radius 

-----

class Circle(object):
    def __init__(self,radius,color):
        self.radius=radius;
        self.color=color;
    
    def addCircle(self,r):
        self.radius=self.radius+r
        
Redcircle=Circle(10,'blue')
Redcircle.addCircle(10)
Redcircle.radius


## Output : 20

```

- methods to change data attribute
- .drawCircle()
- .drawRectangle()
- dir(nameoftheobject): ~~ list of the object data attributes
```
# Import the library

import matplotlib.pyplot as plt
%matplotlib inline  
-------

class Vehicle:
    color = "white"

    def __init__(self, max_speed, mileage):
        self.max_speed = max_speed
        self.mileage = mileage
        self.seating_capacity = None

    def assign_seating_capacity(self, seating_capacity):
        self.seating_capacity = seating_capacity

    def display_properties(self):
        print("Properties of the Vehicle:")
        print("Color:", self.color)
        print("Maximum Speed:", self.max_speed)
        print("Mileage:", self.mileage)
        print("Seating Capacity:", self.seating_capacity)

# Creating objects of the Vehicle class
vehicle1 = Vehicle(200, 50000)
vehicle1.assign_seating_capacity(5)
vehicle1.display_properties()

vehicle2 = Vehicle(180, 75000)
vehicle2.assign_seating_capacity(4)
vehicle2.display_properties()



```


## WEEK 3 DONE 
~~ Soumyajeet Bal






 
