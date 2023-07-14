## Types
- Integer(int), float(float), String(str)
- Integer (negative and positive)
- float are real number which has a decimal place(more accuraacy)
- typecasting (converting one datatype to another)
- loose information during type casting

In type casting, a data type is converted into another data type by a programmer using casting operator. 
Whereas in type conversion, a data type is converted into another data type by a compiler.

- Boolean(bool)
- true - 1
- false - 0

```Text Type:	str
Numeric Types:	int, float, complex
Sequence Types:	list, tuple, range
Mapping Type:	dict
Set Types:	set, frozenset
Boolean Type:	bool
Binary Types:	bytes, bytearray, memoryview
None Type:	NoneType
```
## Expressions and Variables
- the combination of operand and operator to evaluate.
- +, -, * , /
- // integer division
- () > then operators
- variables to store value

## Exercise
- print('Hello, Python!')
```
import sys
print(sys.version)  
```
- #to write comments
- Name error and syntax error, ValueError
- Python is what is called an interpreted language. Compiled languages examine your entire program at compile time, and are able to warn you about a whole class of errors prior to execution.
- In contrast, Python interprets your script line by line as it executes it. Python will stop executing the entire program when it encounters an error (unless the error is expected and handled by the programmer, a more advanced subject that we'll cover later on in this course
- Shift+ enter to execute in jupyter notebook
- operator precedence

## String Operations
- String is a sequence of characters
- ordered sequence
- 0 1 2 3 .. based indexing
- ... -3, -2, -1 based indexing (the first element is the negative length of the string)
- len('dajksbd')
- name="Michael jackson"
- Name[::2]:"McalJcsn"  (every 2nd variable)
- string stride(increment value) and slicing
- Name[0:5:2] (every 2nd value up to index 4) [starting: exclusive ending: increment value]
- + for concatination
- 3*'Hello'
- string is immutable
- \ represents the beginning of the escape sequence
- \n (output in a new line)
- \t (tab space)
- \\ prints a backslash
- r"Hello \ haha" (prints as it is ) (r denotes raw string)
- String Methods (Sequence method and string methods)
- A.upper() (converts all to Uppercase)
- B= A.replace('Michael','Janet')   ~ replace substring in a string
- A.find('el')  ~~ finds substring starting index (output -1 if not found)






























