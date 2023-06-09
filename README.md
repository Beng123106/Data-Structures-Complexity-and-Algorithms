# Matrices and List Comprehension
* A matrix is a representation of numbers, symbols, or expressions in a 2 dimensional array
* in python, matrixes are made using a list in a list. External modules will be imported to help create these 
* there is no actual matrix data type in python, so we just have to create a list within a list that follows the behaviours of a matrix

## Rules for a matrix:  
- All rows must have the same number of values
- All columns must have the same number of values
- All items in the 2D List must have the same data types
- Since indexing always starts at 0 ... row 1 is technically located at matrix_A[0]

* "List comprehension in Python is a concise way of creating lists from the ones that already exist. It provides a shorter syntax to create new lists from existing lists and their values." - Google
```python 
squares = [i**2 for i in range(10)]

print('Our new result: %s' % squares)
```

### List comprehension consists of:

- A Square Bracket containing an expression that describes the list
- One or more For clause to explain its members
- Then a zero or more if clauses depending on the complexity of the list  

# Map and Filter
## map is a built in function that works by applying a function to iterable data (lists). For example:  
```python
def square(num):
    ''' squares the given num argument '''
    return num ** 2
# end of square

array = list(range(1,11))
square_array = list(map(square, array))

print('Original Array:', array)
print('Array Squared:', square_array)
```
* The map function works by performing the square function to each value in 'array'. It is like in math how you have f(g(x))

```python
def upper(x):
    ''' upper() turns string x into its uppercased counter part '''
    return x.upper()

word = 'hello world!'
upper_word = ''.join(list(map(upper, word)))

print(word)
print(upper_word)
```
* The following code is a good example of how map is not always necessary, and before using map consider any much easier, simpler ways to do the same thing. For example, you could have just used word.upper()

### Filter Function
* the function provided for filter() must return a boolean value
* Example of how it works:
```python 
 def isOdd(x):
    ''' isOdd() returns True if x is odd.'''
    return x % 2 != 0

array = list(range(1,101))
odds = list(filter(isOdd, array))
```
# Sets
* a set is an unordered collection with no duplicates
* Why do we even use sets? In computer memory, it creates unique memory adresses for each value in the set. Since every item has unique adresses, if you look for a value in the set it will go directly to that memory adress instead of check each individual value to see if it exists (like it does for a list).
* sets are useful for answering "is this in my data set?" efficiently
* denoted with {}
* a set does not need to be ordered
* duplicate values are disregarded (will be considered as only showing once)
* Union function just adds 2 sets into one
* Intersection function finds overlapping datas between 2 sets
* You can subtract sets A-B takes overlapping values from B away from A
* Symmetric difference is like the opposite of intersection, to find values that dont overlap
* set comprehension exists just like list comprehension

# Dictionary
* data type that stores a collectiom of (key, value) pairs such that each possible key appears at most one time
* common operations are aadding, removing, modifying, lookup a value associated with a particular key
## why are dictionaries useful?
* our index, called keys, doesnt need to be ordered  

* if you want your item in a special location, you can
* to create a dictionary you use dict/empty curly braces {}
* 



