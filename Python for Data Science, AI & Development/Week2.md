## List and Tuples
- these are called compound datatypes
- tuples are ordered sequence
- (values,values,values) ~~ values can be of any data type but the type of the variable is a tuple
- tuple are also zero-based indexing and can be assessed A[index] ~~ negative indexing same as string
- tuple can be contaminated (value,value) + (value,value) = (value,value,value,value)
- tuple2[0:3] ~ first three tuple elements
- len(tuple2) ~~ length of the tuple
- tuples are immutable ~~ cant be changed once declared
- variable only references the tuple
- new tuple to be create to change it
- sorted(tuple2)
- nested tuple ~~ test=(value,value,(value,value),value)
- test[2][0]
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






