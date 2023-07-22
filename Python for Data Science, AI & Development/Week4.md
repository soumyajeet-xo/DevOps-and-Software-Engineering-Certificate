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

# This practice auto-closes the file
```
- mode a will not create a new file but instead, use the existing file
- same .write

## Loading Data with Pandas
- import panda as pd ~~~ importing a library
- csv_path='file1.csv'
- df=pd.read_csv(csv_path)
- df.head()  ~~ first 5 rows of the data frame
- loading Excel file xlsx in a similar way
- df=pd.read_excel(xlsx_path)
- df=pd.DataFrame(songs)  ~~ converts a dictionary into dataframe
- x=df[['Length']] ~~~ dataframe from a new dataframe

## Pandas: Working with and Saving Data
- df['Released'].unique()
- dff['Released']>=1980 ~~ result is a series of boolean values
- df1=df[df['Released']>=1980]
- df1.to_csv('ne_song.csv')

## One Dimensional Numpy
- lib for scientific computing
- basic array creation
- indexing and slicing
- numpy array or nd array is similar to list and usually of fixed size and each element of the same size
- numpy ndarray
- a=np.array([0,1,2,3,4,5,6,7])
- a.size
- a.dtpe -- int64
- a.ndim --- gives dimension
- a.shape -- size of the array in each dimension
- indexing and slicing
- Basic Operations
- vector addition and substraction
- u=np.array([1,0])
- v=np.array([0,1])
- z=u+v
- print(z)
- scalar multiplication
- product of two vectors
- Hadamard product of two vector (simple mutiplication of each component) z=u*v
- dot product (sum of the product of each component) ~~ np.dot(u,v)
- z=u+1 -- 1 will be added to each component -- property is known as broadcasting

```
a=np.array([1,-1,1,-1])
mean_a=a.mean()
max_a=a.max()
pi=np.pi
sin_a=np.sin(a)
line_a=np.linespace(-2,2,num=5)
y=np.linespace(-2,2*np.pi,num=5)
```
## Two-Dimensional Numpy
- Array creation
- indexing and slicing
- a=[[1,2],[2,3]]
- b=np.array(a)
- same function like single dimension numpy


## Week 4 completed
~~ Soumyajeet Bal











