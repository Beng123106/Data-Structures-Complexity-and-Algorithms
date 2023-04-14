# Matrices and List Comprehension
* A matrix is a representation of numbers, symbols, or expressions in a 2 dimensional array
* in python, matrixes are made using a list in a list. External modules will be imported to help create these 
* there is no actual matrix data type in python, so we just have to create a list within a list that follows the behaviours of a matrix

Rules for a matrix:  
- All rows must have the same number of values
- All columns must have the same number of values
- All items in the 2D List must have the same data types
- Since indexing always starts at 0 ... row 1 is technically located at matrix_A[0]

* "List comprehension in Python is a concise way of creating lists from the ones that already exist. It provides a shorter syntax to create new lists from existing lists and their values." - Google
```python 
squares = [i**2 for i in range(10)]

print('Our new result: %s' % squares)
```

List comprehension consists of:

- A Square Bracket containing an expression that describes the list
- One or more For clause to explain its members
- Then a zero or more if clauses depending on the complexity of the list




