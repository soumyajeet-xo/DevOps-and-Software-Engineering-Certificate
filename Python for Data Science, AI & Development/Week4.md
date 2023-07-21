## Reading Files with Open
- open function
- r- reading, w-writing, a-appending
- File1=open("/path","r")
- File1.name
- File1.mode
- File1.close()
-
```
with open("/path/name","r") as File1:
 file_stuff=File1.read()
 print(file_stuff)

# this practice auto closes the file
```
- File1.read(), File1.readline(), File1.readlines() ~~~~~arguments can be passed in all.
- for line in File1: print(line)

## Writing Files with Open
- open function to get a file object
- File1=open("/path/name","w")
- File1.write("hello\n") -- each time it is called, it gets written
```
lines=["dadasdas\n","dasdas\n"]
with open("/path/name","w") as File1:
 
 for line in lines:
   File1.write(line)

# this practice auto closes the file
```
- mode a will not create a new file but rather use the existing file
- 








