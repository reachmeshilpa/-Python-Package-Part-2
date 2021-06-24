# -Python-Package-Part-2
Learning by Implementation: Data Types: Numerical | Boolean | Dictionary
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

#---------------------------
BOOLEAN: True False
age = 20
if age> 19:
  print ('Adult')
elif age> 12:
  print ('Teen')
else:
print ('Child')
OUTPUT-> Adult

# Nested if statements
# if...elif....else within any number of if...elif.....else (avoid as it can be confusing)
# indentation is the only way to figure out the level of nesting.
age = 12
if age >= 13:
    if age<=19:
        print('Teen')
    else: 
        print('Adult')
else:
    print('Child')
OUTPUT-> Child

# Combining operatore in if else...
age = 20
if (age>=13) and (age<=19):
    person_type = 'Teen'
elif (age>=0) and (age<=12):
    person_type = 'Child'
else:
    person_type = 'Adult'
  print ('The person is in category:{}'.format(person_type))
                                      -----------------------
  OUTPUT-> The person is in category: Adult

# While loop in Python
used to **iterate over a block of code** 
as long as the test expression/test condition is **true.**


#---------------------------


#----------------------------
# {Dictionary} is an unordered collection of key-value pairs.
One must know the key to retrieve the value.
Used to retrieve data from a huge repository.

# to know the length or number of keys in a dictionary variable
baking = {1:'brownies', 'quiche':'4', 'cookies':'24'}
**print (len(baking))**
OUTPUT-> 3

# to list all the keys in a dictionary variable
print (dictnry variable.keys())
baking = {1:'brownies', 'quiche':'4', 'cookies':'24'}
**print (baking.keys())**
OUTPUT-> dict_keys([1, 'quiche', 'cookies'])

# to list all the values in a dictionary variable
print (dictnry variable.values())
baking = {1:'brownies', 'quiche':'4', 'cookies':'24'}
**print (baking.values())**
OUTPUT-> dict_values(['brownies', '4', '24'])

# to list all the items in a dictionary variable
print (dictnry variable.values())
baking = {1:'brownies', 'quiche':'4', 'cookies':'24'}
**print (baking.items())**
OUTPUT->dict_items([(1, 'brownies'), ('quiche', '4'), ('cookies', '24')])

# 2nd way to list all the items in a dictionary variable but in a COLUMN format
baking = {1:'brownies', 'quiche':'4', 'cookies':'24'}
for key,value in student.items():
print (key,value)
OUTPUT -> ?????NW



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
  
  # 2nd way to update a value, need to use CURLY braces here within curved braces
  variable.update ({'key':'replaced value'})
  baking.update ({1:'brownies', 'quiche':'4', 'cookies':'24'})
  print (baking)
  Previous output before the update--> {1: 'cupcakes', 'quiche': '12', 'cookies': '24'}
  OUTPUT -> {1: 'brownies', 'quiche': '4', 'cookies': '24'}
  
  
  # key can be a number as well
  baking = {1:'cupcakes', 'quiche':'12', 'cookies':'24'}
  print (baking[1])
  
  # Consider I deleted an element and want to show 'none' for it, will use variable.get
del (baking ['cookies'])
print (baking ('cookies'))
OUTPUT: Traceback and type errorr
#But
print (baking.get('cookies'))
OUTPUT -> None

# None was by default, if I instead want to write something and print that say 'Not found'
print (baking.get('deleted key','what i want to print'))
print (baking.get('cookies','Not found'))
OUTPUT -> Not found
# DICTIONARY
#------------------------------
# To retrieve the key of a deleted element into a new variable and to also print the value of the deleted variable as an output
baking = {1:'brownies', 'quiche':'4', 'cookies':'24'}
key to be deleted as a new variable = dictnry variable.pop ('key to be deleted')
quiche = baking.pop('quiche')
print (baking)
OUTPUT-> {1: 'brownies', 'cookies': '24'}
print (quiche)
OUTPUT-> 4



