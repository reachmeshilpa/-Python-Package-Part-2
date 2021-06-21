# -Python-Package-Part-2
Learning by Implementation
# Data types in Python: the kind of or the type of value assigned to a variable/object
'''
  Numerical
    Integer
    Float
    Complex number
  Boolean
    True
    False
  Dictionary
  Set
  Sequence
    String
    List
    Tuple
'''
num1 = 12               # integer data type
num2 = 12.5             # float data type
num3 = 12.5 + 20k       # complex number data type ??? NW

# to know the datatype of a variable, use print ( type())
print (type (num1, num2, num3))

# to check or recheck the type/class of a variable, use isinstance (variablename, classtocheck)
print (‘ Is ’, data3, ‘type of class complex?’, isinstance (data3, complex))
OUTPUT -> Is (100+20j) type of class complex? True

# {Dictionary} is an unordered collection of key-value pairs.
One must know the key to retrieve the value.
Used to retrieve data from a huge repository.

# variable = { 'key':'value' }          used curly braces for the key and value while creating a variable, k and v separated by colon and placed in quotes
dictnry1 = {'key1':'value1', 'key2':'value2'}

# To print a dictionary     print ( variable [key] ) key is not in curly braces, rather KEY IS in STRAIGHT BRACES when PRINTIMG
print (dictnry1 [ 'key1' ])
OUTPUT -> value1

# For the next three manipulations in a dictionary in python, we use STRAIGHT BRACES and not curly
  # to DELETE a dictionary element (element is key and value)
 del (variable ['key'] )
 print (variable)

  # to ADD a NEW ELEMENT
  variable ['key'] = value
  print (variable)
  dictnry1 ['oranges'] = 8
  print (dictnry1)

  # to UPDATE A VALUE in the dictonary
  variable ['key'] = newvalue
  print (variable)
  
