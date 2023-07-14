## List and Tuples
- these are called compound datatypes
- tuples are ordered sequence
- (values,values,values) ~~ values can be of any data type but the type of the variable is a tuple
- tuple are also zero-based indexing and can be assessed A[index] ~~ negative indexing same as string
- tuple can be concatenated (value,value) + (value,value) = (value,value,value,value)
- tuple2[0:3] ~ first three tuple elements
- len(tuple2) ~~ length of the tuple
- tuples are immutable ~~ cant be changed once declared
- variable only references the tuple
- new tuple to be create to change it
- sorted(tuple2)
- nested tuple ~~ test=(value,value,(value,value),value)
- test[2][0]
- genres_tuple.index("disco") ~~ returns first index of disco in genres_tuples
```
A=('Aloo',("Piyaz","dhaniya"),"Pizza")
A[1][1][1]
OUTPUT - 'h'
```
- LIST
- also ordered sequence too represented by square brackets but they are mutable
- list can nested too
- same indexing like 0 based and negative based
- slicing can be done too ~~ L[3:5]
- concatenated and added too.. but list is mutable
- some exclusive mutable function are
- extend ~~ L.extend([val,val])   ~~ original list modified (extend is like adding)
- append is appending as 1 element to the end of the list ~~ L.append([value,value]) : [value,value,[value,value]]
```
L=['hello',2,7]
L.extend('lol')
L
OUTPUT : ['hello', 2, 7, 'l', 'o', 'l']
```
- del(A[0]) ~~ A is a list
- "hello wordl".split()  ~~ give a list of elements seperated by spaces
- 'A,B,C,D'.split(',') ~~~give a list of item sperated by comma(delimiter)
- Aliasing... multiple name referring to the same object
- if A and B reference the same object... upon changing A list B also changes
- so it is bettter to clone B=A[:]
- help(A)
```
fruits = ("apple", "banana", "cherry")

(green, yellow, red) = fruits

print(green) : apple
print(yellow) : banana
print(red) : cherry
```
A list is a sequenced collection of different objects such as integers, strings, and even other lists as well. The address of each element within a list is called an index. An index is used to access and refer to items within a list.


## Dictionaries
- it is a type of collection in python  (key value pair )
- Each key is separated from its value by a colon
- keys are immutable and unique
- values can mutable, and duplicates
- A={1:"Hello",2:"Hi",3:"Bye"}
- A[1] return Hello
- A[3]="Haha" ~~ adds new key value in the dictionary
- del(A[1])  deletes the first key value pair with key =1 
- if 0 in A ~~~ checks if dict have any key 0
- A.keys() will return a list of all the keys
- A.values() will return list of all the values
- A.items() will return a dict_item type of key-value pair
- 
  Exercise : https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMDeveloperSkillsNetwork-PY0101EN-SkillsNetwork/labs/jupyterlite/files/Module_2/PY0101EN-2-4-Dictionaries-20230526-1685059200.jupyterlite.ipynb

- Keys can also be any immutable object such as a tuple:
- both dictionary and set have same declaration.....  var={}
- 


## Sets 
- sets are mutable like list
- Also a type of collection, they are unordered unlike list and tuples
- set  can be defined using multiple duplicate items but it will store unique items only
- A=[] ~~ is a list
- B=set(A) ~~~converts list to set (called type casting)
- set operations
- vein diagram
- setname.add('nda')
- setname.remove("nda")
- 'nda' in setname
- Mathematical operation
- A & B (intersection between two sets)
- A.union(B) ~~ to find union of set A and B
- album_set1.difference(album_set2) 
- A.issubset(B) return true if A is a subset of B
- set(album_set1).issuperset(album_set2)   
- when converting list to set... it also gets sorted alphabetically
- sum(A) gives sum of all the elements
- 

## WEEK 2 DONE
  ~ Soumyajeet Bal










