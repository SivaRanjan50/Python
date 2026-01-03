```
Python is a popular programming language. 
Python can be used on a server to create web applications. 
 ```

 ## What is python
 ```
Python is a popular programming language. It was created by Guido van 
Rossum, and released in 1991. 
It is used for: 
• web development (server-side), 
• software development, 
• mathematics, 
• system scripting. 
 ```

## what can python do? 
```
• Python can be used on a server to create web applications. 
• Python can be used alongside software to create workflows. 
• Python can connect to database systems. It can also read and 
modify files. 
• Python can be used to handle big data and perform complex 
mathematics. 
• Python can be used for rapid prototyping, or for production-ready 
software development. 
```
 
## why Python?
```
• Python works on different platforms (Windows, Mac, Linux, 
Raspberry Pi, etc). 
• Python has a simple syntax similar to the English language. 
• Python has syntax that allows developers to write programs with 
fewer lines than some other programming languages. 
• Python runs on an interpreter system, meaning that code can be 
executed as soon as it is written. This means that prototyping can 
be very quick. 
• Python can be treated in a procedural way, an object-oriented way 
or a functional way.
```

### Good to know
```
• The most recent major version of Python is Python 3, which we 
shall be using in this tutorial. 
• In this tutorial Python will be written in a text editor. It is possible 
to write Python in an Integrated Development Environment, such 
as Thonny, Pycharm, Netbeans or Eclipse which are particularly 
useful when managing larger collections of Python files.
```

### python syntax compared to other programming languages
```python
Python Syntax compared to other 
• Python was designed for readability, and has some similarities to 
the English language with influence from mathematics. 
• Python uses new lines to complete a command, as opposed to 
other programming languages which often use semicolons or 
parentheses. 
• Python relies on indentation, using whitespace, to define scope; 
such as the scope of loops, functions and classes. Other 
programming languages often use curly-brackets for this purpose.

 print("Hello, World!")
```

## python indentation
```python
Indentation refers to the spaces at the beginning of a code line. 
Where in other programming languages the indentation in code is for 
readability only, the indentation in Python is very important. 
Python uses indentation to indicate a block of code. 
 
Example  
if 5 > 2: 
  print("Five is greater than two!") 
 
 
Python has commenting capability for the purpose of in-code 
documentation. 
Python Indentation 
Comments 
Comments start with a #, and Python will render the rest of the line as a 
comment: 
 
Example 
Comments in Python: 
#This is a comment. 
print("Hello, World!")
```

### semicolons( optional, rarely used)
```python
Semicolons are optional in Python. You can write multiple statements on 
one line by separating them with ; but this is rarely used because it 
makes it hard to read: 
Example 
print("Hello"); print("How are you?");  
print("Bye bye!") 
 ```

### Print Text
```python
You have already learned that you can use the print() function to 
display text or output values: 
Example 
print("Hello World!") 
You can use the print() function as many times as you want. Each call 
prints text on a new line by default: 
 
Example 
print("Hello World!") 
print("I am learning Python.") 
print("It is awesome!")
```

### double quotes
```python
Text in Python must be inside quotes. You can use either " double 
quotes or ' single quotes: 
Example 
print("This will work!") 
print('This will also work!')
```

### print without new line
```python
By default, the print() function ends with a new line. 
If you want to print multiple words on the same line, you can use 
the end parameter: 
Example 
print("Hello World!", end=" ") 
print("I will print on the same line.") 
Note that we add a space after end=" " for better readability. 
print(3) 
print(358) 
print(50000) 
print(3 + 3) 
print(2 * 5) 
print("I am", 35, "years old.") 
 
 
Double Quotes 
Print Without a New Line
```

### comments
```python
Comments starts with a #, and Python will ignore them: 
 
Example  
#This is a comment 
print("Hello, World!") 
Comments can be placed at the end of a line, and Python will ignore the 
rest of the line: 
Example 
print("Hello, World!") #This is a comment
```
 
## variables
```python
Variables are containers for storing data values. 
```
##### creating a variable
```python
Python has no command for declaring a variable. 
A variable is created the moment you first assign a value to it. 
Example  
x = 5 
y = "John" 
print(x) 
print(y) 
 
Creating Variables 
Creating a Comment  
Variables
```

##### casting
```python
If you want to specify the data type of a variable, this can be done with 
casting. 
Example 
x = str(3)    # x will be '3' 
y = int(3)    # y will be 3 
z = float(3)  # z will be 3.0 
```

##### single or double quotes?
```python
String variables can be declared either by using single or double quotes: 
Example 
x = "John" 
# is the same as 
x = 'John' 
```

##### Case - sensitive
```python
Variable names are case-sensitive. 
Example 
This will create two variables: 
a = 4 
A = "Sally" 
#A will not overwrite a 
```

### variable names
```python
A variable can have a short name (like x and y) or a more descriptive 
name (age, carname, total_volume). 
Rules for Python variables: 
• A variable name must start with a letter or the underscore character 
• A variable name cannot start with a number 
• A variable name can only contain alpha-numeric characters and underscores 
(A-z, 0-9, and _ ) 
• Variable names are case-sensitive (age, Age and AGE are three different 
variables) 
• A variable name cannot be any of the Python keywords. 
Example  
Legal variable names: 
myvar = "John" 
my_var = "John" 
_my_var = "John" 
myVar = "John" 
MYVAR = "John" 
myvar2 = "John" 
 
Example 
Illegal variable names: 
2myvar = "John" 
my-var = "John" 
my var = "John" 
Note :- Remember that variable names are case-sensitive 
```

### Multi Words Variables Names
```
Variable names with more than one word can be difficult to read. 
There are several techniques you can use to make them more readable:
``` 
##### Camel Case 
```python
Each word, except the first, starts with a capital letter: 
myVariableName = "John"
```

##### Pascal Case 
```python
Each word starts with a capital letter: 
MyVariableName = "John"
```

##### Snake Case
```python
Each word is separated by an underscore character: 
my_variable_name = "John" 
```

##### Output Variables 
```python
The print() function is often used to output variables. 
Example  
x = "Python is awesome" 
print(x) 
In the print() function, you output multiple variables, separated by a 
comma: 
Example 
Multi Words Variables Names 
x = "Python" 
y = "is" 
z = "awesome" 
print(x, y, z) 
You can also use the + operator to output multiple variables: 
Example 
x = "Python " 
y = "is " 
z = "awesome" 
print(x + y + z) 
Notice the space character after "Python " and "is ", without them 
the result would be "Pythonisawesome". 
For numbers, the + character works as a mathematical operator: 
Example 
x = 5 
y = 10 
print(x + y) 
```

### Global variable
```python
Variables that are created outside of a function (as in all of the examples 
in the previous pages) are known as global variables. 
Global variables can be used by everyone, both inside of functions and 
outside.
Example  
Create a variable outside of a function, and use it inside the function 
x = "awesome" 
 
def myfunc(): 
  print("Python is " + x) 
Global Variables 
 
myfunc() 
```

### Global keyword
```python
Normally, when you create a variable inside a function, that variable is 
local, and can only be used inside that function. 
To create a global variable inside a function, you can use 
the global keyword. 
Example 
If you use the global keyword, the variable belongs to the global scope: 
 
def myfunc(): 
  global x 
  x = "fantastic" 
 
myfunc() 
 
print("Python is " + x) 
```

### Built in data types
```python
In programming, data type is an important concept. 
Variables can store data of different types, and different types can do 
different things. 
Python has the following data types built-in by default, in these 
categories: 
 
The Global Keyword 
Built -In Data Types 
Text Type: Str 
Numeric Types: int, float, complex 
Sequence Types: list, tuple, range 
Mapping Type: Dict 
Set Types: set, frozenset 
Boolean Type: Bool 
Binary Types: bytes, bytearray 
None Type: NoneType
```
 
### Getting the Data Type 
```python
You can get the data type of any object by using the type() function: 
Example  
Print the data type of the variable x: 
x = 5 
print(type(x))
```

### Type Conversion 
```python
You can convert from one type to another with the int(), float(), 
and complex() methods: 
Example 
Convert from one type to another: 
x = 1    # int 
y = 2.8  # float 
z = 1j   # complex 
 
#convert from int to float: 
a = float(x) 
 
#convert from float to int: 
b = int(y) 
 
#convert from int to complex: 
c = complex(x) 
 
print(a) 
print(b) 
print(c) 
 
print(type(a)) 
print(type(b)) 
print(type(c)) 
Note: You cannot convert complex numbers into another number type. 
 ```

### specif a variable type
```python
There may be times when you want to specify a type on to a variable. 
This can be done with casting. Python is an object-orientated language, 
and as such it uses classes to define data types, including its primitive 
types. 
Casting in python is therefore done using constructor functions:

• int() - constructs an integer number from an integer literal, a float literal (by 
removing all decimals), or a string literal (providing the string represents a 
whole number) 
• float() - constructs a float number from an integer literal, a float literal or a 
string literal (providing the string represents a float or an integer) 
• str() - constructs a string from a wide variety of data types, including strings, 
integer literals and float literals 
Specify a Variable Type 
Example  
Integers: 
x = int(1)   # x will be 1 
y = int(2.8) # y will be 2 
z = int("3") # z will be 3 
Example 
Floats: 
x = float(1)     # x will be 1.0 
y = float(2.8)   # y will be 2.8 
z = float("3")   # z will be 3.0 
w = float("4.2") # w will be 4.2 
Example 
Strings: 
x = str("s1") # x will be 's1' 
y = str(2)    # y will be '2' 
z = str(3.0)  # z will be '3.0' 
```

### multiline strings
```python
You can assign a multiline string to a variable by using three quotes: 
Example 
You can use three double quotes: 
a = """Lorem ipsum dolor sit amet, 
consectetur adipiscing elit, 
sed do eiusmod tempor incididunt 
ut labore et dolore magna aliqua.""" 
print(a) 
Note: in the result, the line breaks are inserted at the same position as in the code. 
Multilne Strings 
```

### String length
```python
To get the length of a string, use the len() function. 
Example 
The len() function returns the length of a string: 
a = "Hello, World!" 
print(len(a)) 
 ```

### Slicing
```python
You can return a range of characters by using the slice syntax. 
Specify the start index and the end index, separated by a colon, to return 
a part of the string. 
Example  
Get the characters from position 2 to position 5 (not included): 
b = "Hello, World!" 
print(b[2:5]) 
Note: The first character has index 0. 
b = "Hello, World!" 
print(b[:5]) 
```

### Negative indexing
```python
Use negative indexes to start the slice from the end of the string: 
Example 
Get the characters: 
From: "o" in "World!" (position -5)
To, but not included: "d" in "World!" (position -2): 
b = "Hello, World!" 
print(b[-5:-2]) 
```

### Upper Case 
```python
Example  
The upper() method returns the string in upper case: 
a = "Hello, World!" 
print(a.upper())
```

### Lower Case 
```python
Example 
The lower() method returns the string in lower case: 
a = "Hello, World!" 
print(a.lower())
```

### Remove Whitespace
```python
Whitespace is the space before and/or after the actual text, and very 
often you want to remove this space. 
Example 
The strip() method removes any whitespace from the beginning 
or the end: 
a = " Hello, World! " 
print(a.strip()) # returns "Hello, World!"
```

### Replace String 
```python
Example 
The replace() method replaces a string with another string: 
a = "Hello, World!" 
print(a.replace("H", "J"))
```

### Split String 
```python
The split() method returns a list where the text between the specified 
separator becomes the list items. 
Example 
The split() method splits the string into substrings if it finds instances 
of the separator: 
a = "Hello, World!" 
print(a.split(",")) # returns ['Hello', ' World!'] 
```

### String concatenation
```python
To concatenate, or combine, two strings you can use the + operator. 
Example  
Merge variable a with variable b into variable c: 
a = "Hello" 
b = "World" 
c = a + b 
print(c) 
Example 
To add a space between them, add a " ": 
a = "Hello" 
b = "World" 
c = a + " " + b 
print(c) 
String Concatenation 
Booleans represent one of two values: True or False. 
```

### boolean values
```python
In programming you often need to know if an expression 
is True or False. 
You can evaluate any expression in Python, and get one of two 
answers, True or False. 
When you compare two values, the expression is evaluated and Python 
returns the Boolean answer: 
Example  
print(10 > 9) 
print(10 == 9) 
print(10 < 9)
```
 
 
Operators are used to perform operations on variables and values. 
In the example below, we use the + operator to add together two values: 
Example  
print(10 + 5) 
Python divides the operators in the following groups: 
• Arithmetic operators 
• Assignment operators 
• Comparison operators 
• Logical operators 
• Identity operators 
• Membership operators 
• Bitwise operators 
                        Boolean Values 
Pyhon Operators 
 
Arithmetic operators are used with numeric values to perform common 
mathematical operations: 
Examples 
Here is an example using different arithmetic operators: 
Example  
x = 15 
y = 4 
 
print(x + y) 
print(x - y) 
print(x * y) 
print(x / y) 
print(x % y) 
print(x ** y) 
print(x // y) 
Division in Python 
Python has two division operators: 
• / - Division (returns a float) 
• // - Floor division (returns an integer) 
 
Assignment operators are used to assign values to variables: 
= x = 5 x = 5 
 
Arithmetics Operators 
 Assignment Operators 
+= x += 3 x = x + 3 
 -= x -= 3 x = x - 3 
 
*= x *= 3 x = x * 3 
 
/= x /= 3 x = x / 3 
 
%= x %= 3 x = x % 3 
 
//= x //= 3 x = x // 3 
 
**= x **= 3 x = x ** 3  
 
 
Comparison operators are used to compare two values: 
Operator Name Example 
 
== Equal x == y 
 
Comparison Operators 
!= Not equal x != y 
 
> Greater than x > y 
 
< Less than x < y 
 
>= Greater than or equal to x >= y 
 
<= Less than or equal to x <= y 
 
 
 
Examples 
Comparison operators return True or False based on the comparison: 
Operator Name Example 
== Equal x == y 
 
!= Not equal x != y 
 
> Greater than x > y 
 
< Less than x < y 
 
>= Greater than or equal to x >= y 
 
<= Less than or equal to x <= y  
 
Example  
x = 5 
y = 3 
 
print(x == y) 
print(x != y) 
print(x > y) 
print(x < y) 
print(x >= y) 
print(x <= y) 
 
 
Logical operators are used to combine conditional statements: 
Operator Description Example 
 
Logical Operators 
and  Returns True if both statements are true x < 5 and  x 
< 10 
 
Or Returns True if one of the statements is true x < 5 or x < 
4 
 
Not Reverse the result, returns False if the result is 
true 
not(x < 5 
and x < 10)  
 
Identity operators are used to compare the objects, not if they are equal, 
but if they are actually the same object, with the same memory location: 
Operator Description Example 
is  Returns True if both variables are the same 
object 
x is y 
 
is not Returns True if both variables are not the same 
object 
x is not y  
 
Example  
The is operator returns True if both variables point to the same object: 
Identity Operators 
x = ["apple", "banana"] 
y = ["apple", "banana"] 
z = x 
 
print(x is z) 
print(x is y) 
print(x == y) 
Example 
The is not operator returns True if both variables do not point to the 
same object: 
x = ["apple", "banana"] 
y = ["apple", "banana"] 
 
print(x is not y) 
Difference Between is and == 
• is - Checks if both variables point to the same object in memory 
• == - Checks if the values of both variables are equal 
• x = [1, 2, 3] 
y = [1, 2, 3] 
 
print(x == y) 
print(x is y) 
Membership Operators 
Membership operators are used to test if a sequence is presented in an 
object: 
Operator Description Exampl 
 
in  Returns True if a sequence with the specified value is 
present in the object 
x in y 
 
not in Returns True if a sequence with the specified value is not 
present in the object 
x not in 
y  
Example  
Check if "banana" is present in a list: 
fruits = ["apple", "banana", "cherry"] 
 
print("banana" in fruits) 
Example 
Check if "pineapple" is NOT present in a list: 
fruits = ["apple", "banana", "cherry"] 
 
print("pineapple" not in fruits) 
Membership in Strings 
The membership operators also work with strings: 
Example 
text = "Hello World" 
 
print("H" in text) 
print("hello" in text) 
print("z" not in text) 
 
 
 
Bitwise operators are used to compare (binary) numbers: 
Operato
r 
Name Description Exampl
e 
&  AND Sets each bit to 1 if both bits are 1 x & y 
 
| OR Sets each bit to 1 if one of two bits is 1 x | y 
 
^ XOR Sets each bit to 1 if only one of two bits is 
1 
x ^ y 
 
~ NOT Inverts all the bits ~x 
 
<< Zero fill left 
shift 
Shift left by pushing zeros in from the right 
and let the leftmost bits fall off 
x << 2 
 
>> Signed right 
shift 
Shift right by pushing copies of the 
leftmost bit in from the left, and let the 
rightmost bits fall off 
x >> 2 
 
Example  
The & operator compares each bit and set it to 1 if both are 1, otherwise 
it is set to 0: 
print(6 & 3) 
Bitwise Operators 
The binary representation of 6 is 0110 
The binary representation of 3 is 0011 
Then the & operator compares the bits and returns 0010, which is 2 in 
decimal. 
 
 
Lists are used to store multiple items in a single variable. 
Lists are one of 4 built-in data types in Python used to store collections 
of data, the other 3 are Tuple, Set, and Dictionary, all with different 
qualities and usage. 
Lists are created using square brackets: 
Example  
Create a List: 
thislist = ["apple", "banana", "cherry"] 
print(thislist) 
List items are ordered, changeable, and allow duplicate values. 
List items are indexed, the first item has index [0], the second item has 
index [1] etc. 
 
 
When we say that lists are ordered, it means that the items have a 
defined order, and that order will not change. 
List 
Ordered 
If you add new items to a list, the new items will be placed at the end of 
the list. 
Note: There are some list methods that will change the order, but in 
general: the order of the items will not change. 
 
Changeable 
The list is changeable, meaning that we can change, add, and remove 
items in a list after it has been created. 
 
Allow Duplicates 
Since lists are indexed, lists can have items with the same value: 
Example 
Lists allow duplicate values: 
thislist = ["apple", "banana", "cherry", "apple", "cherry"] 
print(thislist) 
List Length 
To determine how many items a list has, use the len() function: 
Example 
Print the number of items in the list: 
thislist = ["apple", "banana", "cherry"] 
print(len(thislist)) 
 
 
List items can be of any data type: 
Example 
String, int and boolean data types: 
list1 = ["apple", "banana", "cherry"] 
list2 = [1, 5, 7, 9, 3] 
list3 = [True, False, False] 
A list can contain different data types: 
Example 
A list with strings, integers and boolean values: 
list1 = ["abc", 34, True, 40, "male"] 
 
 
From Python's perspective, lists are defined as objects with the data 
type 'list': 
<class 'list'> 
Example 
What is the data type of a list? 
mylist = ["apple", "banana", "cherry"] 
print(type(mylist)) 
 
 
There are four collection data types in the Python programming 
language: 
List Items – Data Types 
Type() 
Python Collections (Arrays) 
• List is a collection which is ordered and changeable. Allows duplicate 
members. 
• Tuple is a collection which is ordered and unchangeable. Allows duplicate 
members. 
• Set is a collection which is unordered, unchangeable*, and unindexed. No 
duplicate members. 
• Dictionary is a collection which is ordered** and changeable. No duplicate 
members. 
List items are indexed and you can access them by referring to the index 
number: 
Note: The first item has index 0. 
Note: The search will start at index 2 (included) and end at index 5 (not included). 
Note : Remember that the first item has index 0. 
Range of Indexes 
You can specify a range of indexes by specifying where to start and 
where to end the range. 
When specifying a range, the return value will be a new list with the 
specified items. 
Example 
Return the third, fourth, and fifth item: 
thislist = 
["apple", "banana", "cherry", "orange", "kiwi", "melon", "mango"] 
print(thislist[2:5]) 
Example 
Check if "apple" is present in the list: 
thislist = ["apple", "banana", "cherry"] 
if "apple" in thislist: 
  print("Yes, 'apple' is in the fruits list") 
Change Item Value 
To change the value of a specific item, refer to the index number: 
Example= 
Change the second item: 
thislist = ["apple", "banana", "cherry"] 
thislist[1] = "blackcurrant" 
print(thislist) 
Change a Range of Item Values 
To change the value of items within a specific range, define a list with the 
new values, and refer to the range of index numbers where you want to 
insert the new values: 
Example 
Change the values "banana" and "cherry" with the values 
"blackcurrant" and "watermelon": 
thislist = ["apple", "banana", "cherry", "orange", "kiwi", "mango"] 
thislist[1:3] = ["blackcurrant", "watermelon"] 
print(thislist) 
Note: The length of the list will change when the number of items inserted does not 
match the number of items replaced. 
Insert Items 
To insert a new list item, without replacing any of the existing values, we 
can use the insert() method. 
The insert() method inserts an item at the specified index: 
Example 
Insert "watermelon" as the third item: 
thislist = ["apple", "banana", "cherry"] 
thislist.insert(2, "watermelon") 
print(thislist) 
Note: As a result of the example above, the list will now contain 4 items. 
Append Items 
To add an item to the end of the list, use the append() method: 
Example  
Using the append() method to append an item: 
thislist = ["apple", "banana", "cherry"] 
thislist.append("orange") 
print(thislist) 
Insert Items 
To insert a list item at a specified index, use 
the insert() method.The insert() method inserts an item at the 
specified index: 
Example 
Insert an item as the second position: 
thislist = ["apple", "banana", "cherry"] 
thislist.insert(1, "orange") 
print(thislist) 
Note: As a result of the examples above, the lists will now contain 4 items. 
Remove Specified Item 
The remove() method removes the specified item. 
Example Remove "banana": 
thislist = ["apple", "banana", "cherry"] 
thislist.remove("banana") 
print(thislist) 
If there are more than one item with the specified value, 
the remove() method removes the first occurrence: 
Example 
Remove the first occurrence of "banana": 
thislist = ["apple", "banana", "cherry", "banana", "kiwi"] 
thislist.remove("banana") 
print(thislist) 
Remove Specified Index 
The pop() method removes the specified index. 
Example 
Remove the second item: 
thislist = ["apple", "banana", "cherry"] 
thislist.pop(1) 
print(thislist) 
If you do not specify the index, the pop() method removes the last item. 
Example 
Remove the last item: 
thislist = ["apple", "banana", "cherry"] 
thislist.pop() 
print(thislist) 
The del keyword also removes the specified index: 
Example 
Remove the first item: 
thislist = ["apple", "banana", "cherry"] 
del thislist[0] 
print(thislist) 
The del keyword can also delete the list completely. 
Example 
Delete the entire list: 
thislist = ["apple", "banana", "cherry"] 
del thislist 
The clear() method empties the list. 
The list still remains, but it has no content. 
Example 
Clear the list content: 
thislist = ["apple", "banana", "cherry"] 
thislist.clear() 
print(thislist) 
 
You can loop through the list items by using a for loop: 
Example  
Print all items in the list, one by one: 
thislist = ["apple", "banana", "cherry"] 
for x in thislist: 
  print(x) 
 
You can also loop through the list items by referring to their index 
number. 
Loop Through a List 
Loop Through The Index Number   
Use the range() and len() functions to create a suitable iterable. 
Example 
Print all items by referring to their index number: 
thislist = ["apple", "banana", "cherry"] 
for i in range(len(thislist)): 
  print(thislist[i]) 
 
List objects have a sort() method that will sort the list 
alphanumerically, ascending, by default: 
Example  
Sort the list alphabetically: 
thislist = ["orange", "mango", "kiwi", "pineapple", "banana"] 
thislist.sort() 
print(thislist) 
Example 
Sort the list numerically: 
thislist = [100, 50, 65, 82, 23] 
thislist.sort() 
print(thislist) 
 
To sort descending, use the keyword argument reverse = True: 
Example 
Sort the list descending: 
thislist = ["orange", "mango", "kiwi", "pineapple", "banana"] 
thislist.sort(reverse = True) 
print(thislist) 
 
 
Sort List Alphanumerically 
Sort Descending  
 
 
You cannot copy a list simply by typing list2 = list1, 
because: list2 will only be a reference to list1, and changes made 
in list1 will automatically also be made in list2. 
 
You can use the built-in List method copy() to copy a list. 
Example  
Make a copy of a list with the copy() method: 
thislist = ["apple", "banana", "cherry"] 
mylist = thislist.copy() 
print(mylist) 
There are several ways to join, or concatenate, two or more lists in 
Python. 
One of the easiest ways are by using the + operator. 
Example  
Join two list: 
list1 = ["a", "b", "c"] 
list2 = [1, 2, 3] 
 
list3 = list1 + list2 
print(list3) 
Another way to join two lists is by appending all the items from list2 into 
list1, one by one: 
Copy a List 
Example 
Append list2 into list1: 
list1 = ["a", "b" , "c"] 
list2 = [1, 2, 3] 
 
for x in list2: 
  list1.append(x) 
 
print(list1) 
 
Python has a set of built-in methods that you can use on lists. 
Method Description 
append() Adds an element at the end of the list 
clear() Removes all the elements from the list 
copy() Returns a copy of the list 
count() Returns the number of elements with the specified value 
extend() Add the elements of a list (or any iterable), to the end of the current 
list 
List Methods  
index() Returns the index of the first element with the specified value 
insert() Adds an element at the specified position 
pop() Removes the element at the specified position 
remove() Removes the 
I                                                                                                                                                                                                                                                         
tem with the specified value 
reverse() Reverses the order of the list 
                                                                                                                                                                                                                                                          
sort() 
Sorts the list 
                                                                                                                             
Tuples are used to store multiple items in a single variable. 
Tuple is one of 4 built-in data types in Python used to store collections 
of data, the other 3 are List, Set, and Dictionary, all with different 
qualities and usage. 
A tuple is a collection which is ordered and unchangeable. 
Tuples are written with round brackets. 
Example  
Create a Tuple: 
Tuple Items 
thistuple = ("apple", "banana", "cherry") 
print(thistuple) 
 
Tuple items are ordered, unchangeable, and allow duplicate values. 
Tuple items are indexed, the first item has index [0], the second item 
has index [1] etc. 
 
When we say that tuples are ordered, it means that the items have a 
defined order, and that order will not change. 
 
 
Tuples are unchangeable, meaning that we cannot change, add or 
remove items after the tuple has been created. 
 
 
Since tuples are indexed, they can have items with the same value: 
Example 
Tuples allow duplicate values: 
thistuple = ("apple", "banana", "cherry", "apple", "cherry") 
print(thistuple) 
 
Once a tuple is created, you cannot change its values. Tuples 
are unchangeable, or immutable as it also is called. 
Ordered 
                          Unchangeable 
Allow Duplicates 
Change Tuple values 
But there is a workaround. You can convert the tuple into a list, change 
the list, and convert the list back into a tuple. 
Example  
Convert the tuple into a list to be able to change it: 
x = ("apple", "banana", "cherry") 
y = list(x) 
y[1] = "kiwi" 
x = tuple(y) 
 
print(x) 
 
Since tuples are immutable, they do not have a built
in append() method, but there are other ways to add items to a tuple. 
1. Convert into a list: Just like the workaround for changing a tuple, you 
can convert it into a list, add your item(s), and convert it back into a 
tuple. 
Example 
Convert the tuple into a list, add "orange", and convert it back into 
a tuple: 
thistuple = ("apple", "banana", "cherry") 
y = list(thistuple) 
y.append("orange") 
thistuple = tuple(y) 
2. Add tuple to a tuple. You are allowed to add tuples to tuples, so if 
you want to add one item, (or many), create a new tuple with the 
item(s), and add it to the existing tuple: 
Example 
Create a new tuple with the value "orange", and add that tuple: 
thistuple = ("apple", "banana", "cherry") 
y = ("orange",) 
Add Items 
thistuple += y 
print(thistuple) 
Note: When creating a tuple with only one item, remember to include a 
comma after the item, otherwise it will not be identified as a tuple. 
Remove Items 
Note: You cannot remove items in a tuple. 
Tuples are unchangeable, so you cannot remove items from it, but you 
can use the same workaround as we used for changing and adding tuple 
items: 
Example 
Convert the tuple into a list, remove "apple", and convert it back 
into a tuple: 
thistuple = ("apple", "banana", "cherry") 
y = list(thistuple) 
y.remove("apple") 
thistuple = tuple(y) 
 
Sets are used to store multiple items in a single variable. 
Set is one of 4 built-in data types in Python used to store collections of 
data, the other 3 are List, Tuple, and Dictionary, all with different qualities 
and usage. 
A set is a collection which is unordered, unchangeable*, and unindexed. 
* Note: Set items are unchangeable, but you can remove items and add 
new items. 
Sets are written with curly brackets. 
Set 
Example  
Create a Set: 
thisset = {"apple", "banana", "cherry"} 
print(thisset) 
Note: Sets are unordered, so you cannot be sure in which order the items will 
appear. 
 
Set items are unordered, unchangeable, and do not allow duplicate 
values. 
 
Unordered means that the items in a set do not have a defined order. 
Set items can appear in a different order every time you use them, and 
cannot be referred to by index or key. 
 
Set items are unchangeable, meaning that we cannot change the items 
after the set has been created. 
Once a set is created, you cannot change its items, but you can remove 
items and add new items. 
 
Sets cannot have two items with the same value. 
Example 
Duplicate values will be ignored: 
thisset = {"apple", "banana", "cherry", "apple"} 
 
print(thisset) 
Set Items  
                           Unordered 
Unchangeable 
Duplicates Not Allowed 
Note: The values True and 1 are considered the same value in sets, and 
are treated as duplicates: 
Example 
True and 1 is considered the same value: 
thisset = {"apple", "banana", "cherry", True, 1, 2} 
 
print(thisset) 
Note: The values False and 0 are considered the same value in sets, and 
are treated as duplicates: 
Example 
False and 0 is considered the same value: 
thisset = {"apple", "banana", "cherry", False, True, 0} 
 
print(thisset) 
 
There are four collection data types in the Python programming 
language: 
• List is a collection which is ordered and changeable. Allows duplicate 
members. 
• Tuple is a collection which is ordered and unchangeable. Allows duplicate 
members. 
• Set is a collection which is unordered, unchangeable*, and unindexed. No 
duplicate members. 
• Dictionary is a collection which is ordered** and changeable. No duplicate 
members. 
Access Items 
You cannot access items in a set by referring to an index or a key. 
But you can loop through the set items using a for loop, or ask if a 
specified value is present in a set, by using the in keyword. 
             Python Collections (Arrays) 
Example  
Loop through the set, and print the values: 
thisset = {"apple", "banana", "cherry"} 
 
for x in thisset: 
  print(x) 
Example 
Check if "banana" is present in the set: 
thisset = {"apple", "banana", "cherry"} 
 
print("banana" in thisset) 
Add Items 
Once a set is created, you cannot change its items, but you can add new 
items. 
To add one item to a set use the add() method. 
Example  
Add an item to a set, using the add() method: 
thisset = {"apple", "banana", "cherry"} 
 
thisset.add("orange") 
 
print(thisset) 
Add Sets 
To add items from another set into the current set, use 
the update() method. 
Example 
Add elements from tropical into thisset: 
thisset = {"apple", "banana", "cherry"} 
tropical = {"pineapple", "mango", "papaya"} 
 
thisset.update(tropical) 
 
print(thisset) 
Remove Item 
To remove an item in a set, use the remove(), or 
the discard() method. 
Example  
Remove "banana" by using the remove() method: 
thisset = {"apple", "banana", "cherry"} 
 
thisset.remove("banana") 
 
print(thisset) 
Note: If the item to remove does not exist, remove() will raise an error. 
Example 
Remove "banana" by using the discard() method: 
thisset = {"apple", "banana", "cherry"} 
 
thisset.discard("banana") 
 
print(thisset) 
Note: If the item to remove does not exist, discard() will NOT raise an 
error. 
You can also use the pop() method to remove an item, but this method 
will remove a random item, so you cannot be sure what item that gets 
removed. 
The return value of the pop() method is the removed item. 
Example 
Remove a random item by using the pop() method: 
thisset = {"apple", "banana", "cherry"} 
 
x = thisset.pop() 
 
print(x) 
 
print(thisset) 
Note: Sets are unordered, so when using the pop() method, you do not know which 
item that gets removed. 
 
You can loop through the set items by using a for loop: 
Example  
Loop through the set, and print the values: 
thisset = {"apple", "banana", "cherry"} 
 
for x in thisset: 
  print(x) 
 
 
Dictionaries are used to store data values in key:value pairs. 
A dictionary is a collection which is ordered*, changeable and do not 
allow duplicates. 
As of Python version 3.7, dictionaries are ordered. In Python 3.6 and 
earlier, dictionaries are unordered. 
Dictionaries are written with curly brackets, and have keys and values: 
Example  
Create and print a dictionary: 
Loop Items 
Dictionary 
thisdict = { 
  "brand": "Ford", 
  "model": "Mustang", 
  "year": 1964 
} 
print(thisdict) 
 
 
Dictionary items are ordered, changeable, and do not allow duplicates. 
Dictionary items are presented in key:value pairs, and can be referred to 
by using the key name. 
Example 
Print the "brand" value of the dictionary: 
thisdict = { 
  "brand": "Ford", 
  "model": "Mustang", 
  "year": 1964 
} 
print(thisdict["brand"]) 
 
 
As of Python version 3.7, dictionaries are ordered. In Python 3.6 and 
earlier, dictionaries are unordered. 
When we say that dictionaries are ordered, it means that the items have 
a defined order, and that order will not change. 
Unordered means that the items do not have a defined order, you 
cannot refer to an item by using an index. 
 
 
 
                    Dictionary Items  
Ordered or Unordered? 
 
Dictionaries are changeable, meaning that we can change, add or 
remove items after the dictionary has been created. 
 
Dictionaries cannot have two items with the same key: 
Example 
Duplicate values will overwrite existing values: 
thisdict = { 
  "brand": "Ford", 
  "model": "Mustang", 
  "year": 1964, 
  "year": 2020 
} 
print(thisdict) 
Accessing Items 
You can access the items of a dictionary by referring to its key name, 
inside square brackets: 
Example  
Get the value of the "model" key: 
thisdict = { 
  "brand": "Ford", 
  "model": "Mustang", 
  "year": 1964 
} 
x = thisdict["model"] 
Changeable 
Change Values 
You can change the value of a specific item by referring to its key 
name: 
Example  
Change the "year" to 2018: 
thisdict = { 
  "brand": "Ford", 
  "model": "Mustang", 
  "year": 1964 
} 
thisdict["year"] = 2018 
Update Dictionary 
The update() method will update the dictionary with the items from the 
given argument. 
The argument must be a dictionary, or an iterable object with key:value 
pairs. 
Example 
Update the "year" of the car by using the update() method: 
thisdict = { 
  "brand": "Ford", 
  "model": "Mustang", 
  "year": 1964 
} 
thisdict.update({"year": 2020}) 
Adding Items 
Adding an item to the dictionary is done by using a new index key and 
assigning a value to it: 
Example  
thisdict = { 
  "brand": "Ford", 
  "model": "Mustang", 
  "year": 1964 
} 
thisdict["color"] = "red" 
print(thisdict) 
Update Dictionary 
The update() method will update the dictionary with the items from a 
given argument. If the item does not exist, the item will be added. 
The argument must be a dictionary, or an iterable object with key:value 
pairs. 
Example 
Add a color item to the dictionary by using the update() method: 
thisdict = { 
  "brand": "Ford", 
  "model": "Mustang", 
  "year": 1964 
} 
thisdict.update({"color": "red"}) 
Removing Items 
There are several methods to remove items from a dictionary: 
Example  
The pop() method removes the item with the specified key name: 
thisdict = { 
  "brand": "Ford", 
  "model": "Mustang", 
  "year": 1964 
} 
thisdict.pop("model") 
print(thisdict) 
Example 
The popitem() method removes the last inserted item (in versions 
before 3.7, a random item is removed instead): 
thisdict = { 
  "brand": "Ford", 
  "model": "Mustang", 
  "year": 1964 
} 
thisdict.popitem() 
print(thisdict) 
Example 
The del keyword removes the item with the specified key name: 
thisdict = { 
  "brand": "Ford", 
  "model": "Mustang", 
  "year": 1964 
} 
del thisdict["model"] 
print(thisdict) 
Loop Through a Dictionary 
You can loop through a dictionary by using a for loop. 
When looping through a dictionary, the return value are the keys of the 
dictionary, but there are methods to return the values as well. 
Example  
Print all key names in the dictionary, one by one: 
for x in thisdict: 
  print(x) 
Example 
Print all values in the dictionary, one by one: 
for x in thisdict: 
  print(thisdict[x]) 
Example 
You can also use the values() method to return values of a 
dictionary: 
for x in thisdict.values(): 
  print(x) 
Example 
You can use the keys() method to return the keys of a dictionary: 
for x in thisdict.keys(): 
  print(x) 
Example 
Loop through both keys and values, by using the items() method: 
for x, y in thisdict.items(): 
  print(x, y) 
You cannot copy a dictionary simply by typing dict2 = dict1, 
because: dict2 will only be a reference to dict1, and changes made 
in dict1 will automatically also be made in dict2. 
There are ways to make a copy, one way is to use the built-in Dictionary 
method copy(). 
Example  
Make a copy of a dictionary with the copy() method: 
thisdict = { 
  "brand": "Ford", 
  "model": "Mustang", 
  "year": 1964 
} 
mydict = thisdict.copy() 
print(mydict) 
Another way to make a copy is to use the built-in function dict(). 
Example 
Make a copy of a dictionary with the dict() function: 
thisdict = { 
  "brand": "Ford", 
  "model": "Mustang", 
  "year": 1964 
} 
mydict = dict(thisdict) 
print(mydict) 
 
 
A dictionary can contain dictionaries, this is called nested dictionaries. 
ExampleGet your own Python Server 
Create a dictionary that contain three dictionaries: 
myfamily = { 
  "child1" : { 
    "name" : "Emil", 
    "year" : 2004 
  }, 
  "child2" : { 
    "name" : "Tobias", 
    "year" : 2007 
  }, 
  "child3" : { 
    "name" : "Linus", 
    "year" : 2011 
  } 
} 
To access items from a nested dictionary, you use the name of the 
dictionaries, starting with the outer dictionary: 
Nested Dictionaries 
Example 
Print the name of child 2: 
print(myfamily["child2"]["name"]) 
 
Python has a set of built-in methods that you can use on 
dictionaries. 
Method Description 
clear() Removes all the elements from the dictionary 
copy() Returns a copy of the dictionary 
fromkeys() Returns a dictionary with the specified keys and value 
get() Returns the value of the specified key 
items() Returns a list containing a tuple for each key value pair 
keys() Returns a list containing the dictionary's keys 
pop() Removes the element with the specified key 
Dictionary Methods 
popitem() Removes the last inserted key-value pair 
setdefault() Returns the value of the specified key. If the key does not exist: insert the 
key, with the specified value 
update() Updates the dictionary with the specified key-value pairs 
values() Returns a list of all the values in the dictionary 
 
Python supports the usual logical conditions from mathematics: 
• Equals: a == b 
• Not Equals: a != b 
• Less than: a < b 
• Less than or equal to: a <= b 
• Greater than: a > b 
• Greater than or equal to: a >= b 
These conditions can be used in several ways, most commonly in "if 
statements" and loops. 
An "if statement" is written by using the if keyword. 
a = 33 
b = 200 
if b > a: 
  print("b is greater than a") 
 
Python Conditions and If Statements 
The Elif Keyword 
The elif keyword is Python's way of saying "if the previous conditions 
were not true, then try this condition". 
The elif keyword allows you to check multiple expressions for True and 
execute a block of code as soon as one of the conditions evaluates 
to True. 
Example  
a = 33 
b = 33 
if b > a: 
  print("b is greater than a") 
elif a == b: 
  print("a and b are equal") 
 
 
You can have as many elif statements as you need. Python will check 
each condition in order and execute the first one that is true. 
Example 
Testing multiple conditions: 
score = 75 
 
if score >= 90: 
  print("Grade: A") 
elif score >= 80: 
  print("Grade: B") 
elif score >= 70: 
  print("Grade: C") 
elif score >= 60: 
  print("Grade: D") 
 
 
Multiple Elif Statements 
Match (Switch- Case) 
The match statement is used to perform different actions based on 
different conditions. 
 
 
Instead of writing many if..else statements, you can use 
the match statement. 
The match statement selects one of many code blocks to be executed. 
day = 4 
match day: 
  case 6: 
    print("Today is Saturday") 
  case 7: 
    print("Today is Sunday") 
  case _: 
    print("Looking forward to the Weekend") 
 
 
Python has two primitive loop commands: 
• while loops 
• for loops 
 
With the while loop we can execute a set of statements as long as a 
condition is true. 
Example  
Print i as long as i is less than 6: 
i = 1 
while i < 6: 
The Python Match Statements 
                                   Loops  
The While Loop 
  print(i) 
  i += 1 
 
Note: remember to increment i, or else the loop will continue forever. 
 
With the break statement we can stop the loop even if the while 
condition is true: 
Example 
Exit the loop when i is 3: 
i = 1 
while i < 6: 
  print(i) 
  if i == 3: 
    break 
  i += 1 
 
 
With the continue statement we can stop the current iteration, and 
continue with the next: 
Example 
Continue to the next iteration if i is 3: 
i = 0 
while i < 6: 
  i += 1 
  if i == 3: 
    continue 
  print(i) 
A for loop is used for iterating over a sequence (that is either a list, a tuple, a 
dictionary, a set, or a string). 
Example  
           The Break Statement 
               The Continue Statements 
Print each fruit in a fruit list: 
fruits = ["apple", "banana", "cherry"] 
for x in fruits: 
  print(x) 
 
To loop through a set of code a specified number of times, we can use 
the range() function, 
The range() function returns a sequence of numbers, starting from 0 by 
default, and increments by 1 (by default), and ends at a specified 
number. 
Example 
Using the range() function: 
for x in range(6): 
  print(x) 
Note that range(6) is not the values of 0 to 6, but the values 0 to 5. 
Example 
Using the start parameter: 
for x in range(2, 6): 
  print(x) 
Example 
Increment the sequence with 3 (default is 1): 
for x in range(2, 30, 3): 
  print(x) 
 
A nested loop is a loop inside a loop. 
                   The range() Function  
                             Nested Loops 
The "inner loop" will be executed one time for each iteration of the 
"outer loop": 
Example 
Print each adjective for every fruit: 
adj = ["red", "big", "tasty"] 
fruits = ["apple", "banana", "cherry"] 
 
for x in adj: 
  for y in fruits: 
    print(x, y) 
 
 
A function is a block of code which only runs when it is called. 
A function can return data as a result. 
A function helps avoiding code repetition. 
 
In Python, a function is defined using the def keyword, followed by a 
function name and parentheses: 
Example  
def my_function(): 
  print("Hello from a function") 
my_function() 
my_function() 
my_function() 
 
Function names follow the same rules as variable names in Python: 
• A function name must start with a letter or underscore 
                        Functions 
             Creating a Function 
             Function Names  
• A function name can only contain letters, numbers, and 
underscores 
• Function names are case-sensitive (myFunction and myfunction are 
different) 
Example 
Valid function names: 
calculate_sum() 
_private_function() 
myFunction2() 
It's good practice to use descriptive names that explain what the function does. 
 
The terms parameter and argument can be used for the same thing: 
information that are passed into a function. 
From a function's perspective: 
A parameter is the variable listed inside the parentheses in the function 
definition. 
An argument is the actual value that is sent to the function when it is 
called. 
Example 
def my_function(name): # name is a parameter 
  print("Hello", name) 
 
my_function("Emil") # "Emil" is an argument 
 
You can assign default values to parameters. If the function is called 
without an argument, it uses the default value: 
Parameters vs Arguments 
Default Parameter Values 
Example 
def my_function(name = "friend"): 
  print("Hello", name) 
 
my_function("Emil") 
my_function("Tobias") 
my_function() 
my_function("Linus") 
 
 
1) Function Without Parameter Without Return 
Type 
2) Function With Parameter Without Return Type 
3) Function With Parameter With Return Type 
4) Function With Parameter With Return Type 
 
                                     
 
A variable created in the main body of the Python code is a global 
variable and belongs to the global scope. 
Global variables are available from within any scope, global and 
local. 
 
Example 
A variable created outside of a function is global and can be used 
by anyone: 
 
x = 300 
def myfunc(): 
  print(x) 
 
myfunc() 
 
print(x) 
                           Function Types  
                 Global Scopes  
 
 
The built-in range() function returns an immutable sequence of 
numbers, commonly used for looping a specific number of times. 
This set of numbers has its own data type called range. 
Note: Immutable means that it cannot be modified after it is 
created. 
 
Creating ranges 
The range() function can be called with 1, 2, or 3 arguments, using 
this syntax: 
range(start, stop, step) 
 
 
If you need to create a global variable, but are stuck in the 
local scope, you can use the global keyword. 
The global keyword makes the variable global. 
Example 
If you use the global keyword, the variable belongs to the 
global scope: 
def myfunc(): 
  global x 
  x = 300 
 
Python Range  
                          Global Keyword 
myfunc() 
 
print(x) 
The range() function can be called with 1, 2, or 3 arguments, using this 
syntax:
 
range(start, stop, step) 
Call range() With Two Arguments 
If the range function is called with two arguments, the first argument 
represents the start value, and the second argument represents 
the stop value. 
range(3, 10) returns a sequence of each number from 3 to 9: 
Example 
Create a range of numbers from 3 to 9: 
x = range(3, 10) 
Call range() With Three 
Arguments 
If the range function is called with three arguments, the third argument 
represents the step value. 
The step value means the difference between each number in the 
sequence. It is optional, and if not provided, it defaults to 1. 
range(3, 10, 2) returns a sequence of each number from 3 to 9, with 
a step of 2: 
Example 
Create a range of numbers from 3 to 9: 
x = range(3, 10, 2) 
 
 
Ranges are often used in for loops to iterate over a sequence of 
numbers. 
Example 
Iterate over each value in a range: 
for i in range(10): 
  print(i) 
Using List to Display Ranges 
The range object is a data type that represents an immutable sequence 
of numbers, and it is not directly displayable. 
Therefore, ranges are often converted to lists for display. 
Example 
Convert different ranges to lists: 
print(list(range(5))) 
print(list(range(1, 6))) 
print(list(range(5, 20, 3))) 
 
 
                              Using  Range  
                             Slicing  Ranges  
Like other sequences, ranges can be sliced to extract a subsequence. 
Example 
Extract a subsequence from a range: 
r = range(10) 
print(r[2]) 
print(r[:3]) 
Length 
Ranges support the len() function to get the number of elements in the 
range. 
ExampleGet the length of a range: 
r = range(0, 10, 2) 
print(len(r)) 
Python Arrays 
 
Note: Python does not have built-in support for Arrays, but Python 
Lists can be used instead. 
 
Arrays 
Note: This page shows you how to use LISTS as ARRAYS, however, to 
work with arrays in Python you will have to import a library, like 
the NumPy library. 
Arrays are used to store multiple values in one single variable: 
Example  
Create an array containing car names: 
cars = ["Ford", "Volvo", "BMW"] 
What is an Array? 
An array is a special variable, which can hold more than one value at a 
time. 
If you have a list of items (a list of car names, for example), storing the 
cars in single variables could look like this: 
car1 = "Ford" 
car2 = "Volvo" 
car3 = "BMW" 
However, what if you want to loop through the cars and find a specific 
one? And what if you had not 3 cars, but 300? 
The solution is an array! 
An array can hold many values under a single name, and you can access 
the values by referring to an index number. 
 
Access the Elements of an Array 
You refer to an array element by referring to the index number. 
Example 
Get the value of the first array item: 
x = cars[0] 
The Length of an Array 
Use the len() method to return the length of an array (the number of 
elements in an array). 
Example 
Return the number of elements in the cars array: 
x = len(cars) 
 
Note: The length of an array is always one more than the highest array index. 
Python Modules 
 
 
 
Consider a module to be the same as a code library. 
A file containing a set of functions you want to include in your 
application. 
 
Create a Module 
               What is a Module ? 
To create a module just save the code you want in a file with the file 
extension .py: 
Example  
Save this code in a file named mymodule.py 
def greeting(name): 
  print("Hello, " + name) 
Use a Module 
Now we can use the module we just created, by using 
the import statement: 
Example 
Import the module named mymodule, and call the greeting function: 
import mymodule 
 
mymodule.greeting("Jonathan") 
Note: When using a function from a module, use the 
syntax: module_name.function_name. 
 
Variables in Module 
The module can contain functions, as already described, but also 
variables of all types (arrays, dictionaries, objects etc): 
Example 
Save this code in the file mymodule.py 
person1 = { 
  "name": "John", 
  "age": 36, 
  "country": "Norway" 
} 
The try block lets you test a block of code for errors. 
The except block lets you handle the error. 
The else block lets you execute code when there is no error. 
The finally block lets you execute code, regardless of the result of the 
try- and except blocks. 
 
When an error occurs, or exception as we call it, Python will normally 
stop and generate an error message. 
These exceptions can be handled using the try statement: 
Example  
The try block will generate an exception, because x is not defined: 
try: 
  print(x) 
except: 
  print("An exception occurred") 
Many Exceptions 
You can define as many exception blocks as you want, e.g. if you want to 
execute a special block of code for a special kind of error: 
Example 
Print one message if the try block raises a NameError and another for 
other errors: 
try: 
  print(x) 
except NameError: 
  print("Variable x is not defined") 
except: 
  print("Something else went wrong") 
Else 
You can use the else keyword to define a block of code to be executed 
if no errors were raised: 
Example 
In this example, the try block does not generate any error: 
try: 
  print("Hello") 
except: 
  print("Something went wrong") 
else: 
  print("Nothing went wrong") 
Finally 
The finally block, if specified, will be executed regardless if the try 
block raises an error or not. 
Example 
try: 
  print(x) 
except: 
  print("Something went wrong") 
finally: 
  print("The 'try except' is finished") 
Python PIP 
 
What is PIP?
PIP is a package manager for Python packages, or modules if you like. 
Note: If you have Python version 3.4 or later, PIP is included by default. 
 
A package contains all the files you need for a module. 
Modules are Python code libraries you can include in your project. 
 
Navigate your command line to the location of Python's script directory, 
and type the following: 
Example  
What is a Package? 
Check if PIP is Installed 
Check PIP version: 
pip --version 
 
 
  
Downloading a package is very easy. 
Open the command line interface and tell PIP to download the package 
you want. 
Navigate your command line to the location of Python's script directory, 
and type the following: 
Example 
Download a package named "camelcase": 
C:\Users\Your Name\AppData\Local\Programs\Python\Python36
32\Scripts>pip install camelcase 
 
Python String Formatting 
 
F-String was introduced in Python 3.6, and is now the preferred way of 
formatting strings. 
Before Python 3.6 we had to use the format() method. 
 
Download a Package 
Python String Formatting 
F-Strings 
F-string allows you to format selected parts of a string. 
To specify a string as an f-string, simply put an f in front of the string 
literal, like this: 
Example  
Create an f-string: 
txt = f"The price is 49 dollars" 
print(txt) 
Placeholders and Modifiers 
To format values in an f-string, add placeholders {}, a placeholder can 
contain variables, operations, functions, and modifiers to format the 
value. 
Example 
Add a placeholder for the price variable: 
price = 59 
txt = f"The price is {price} dollars" 
print(txt) 
Example 
Display the price with 2 decimals: 
price = 59 
txt = f"The price is {price:.2f} dollars" 
print(txt) 
txt = f"The price is {20 * 59} dollars" 
print(txt) 
Example 
Add taxes before displaying the price: 
price = 59 
tax = 0.25 
txt = f"The price is {price + (price * tax)} dollars" 
print(txt) 
Python None 
 
None is a special constant in Python that represents the absence of a 
value. 
Its data type is NoneType, and None is the only instance of 
a NoneType object. 
 
Variables can be assigned None to indicate "no value" or "not set". 
Example  
Assign and display a None value: 
x = None 
print(x) 
Use type() to see the type of a None value. 
Example 
Assign and print the data type of a None value: 
x = None 
print(type(x)) 
Python User Input 
 
User Input 
Python allows for user input. 
That means we are able to ask the user for input. 
The following example asks for your name, and when you enter a name, 
it gets printed on the screen: 
Example  
Ask for user input: 
print("Enter your name:") 
name = input() 
print(f"Hello {name}") 
Python stops executing when it comes to the input() function, and continues when 
the user has given some input. 
Multiple Inputs 
You can add as many inputs as you want, Python will stop executing at 
each of them, waiting for user input: 
Example 
Multiple inputs: 
name = input("Enter your name:") 
print(f"Hello {name}") 
fav1 = input("What is your favorite animal:") 
fav2 = input("What is your favorite color:") 
fav3 = input("What is your favorite number:") 
print(f"Do you want a {fav2} {fav1} with {fav3} legs?") 
 
Python Datetime 
 
A date in Python is not a data type of its own, but we can import a 
module named datetime to work with dates as date objects. 
Example  
Import the datetime module and display the current date: 
import datetime 
 
x = datetime.datetime.now() 
print(x) 
Example 
Return the year and name of weekday: 
import datetime 
 
x = datetime.datetime.now() 
 
print(x.year) 
print(x.strftime("%A")) 
 
Directive 
 
Description 
 
Example 
 
%a Weekday, short version Wed 
 
%A Weekday, full version Wednesday 
 
%w Weekday as a number 0-6, 0 is Sunday 3 
 
%d Day of month 01-31 31 
 
%b Month name, short version Dec 
 
%B Month name, full version December 
 
%m Month as a number 01-12 12 
 
%y Year, short version, without century 18 
 
%Y Year, full version 2018 
 
%p AM/PM PM 
 
%f Microsecond 000000-999999 548513 
 
%z UTC offset +0100 
 
%Z Timezone CST 
 
%j Day number of year 001-366 365 
 
%U Week number of year, Sunday as the first day of 
week, 00-53 
52 
 
%W Week number of year, Monday as the first day 
of week, 00-53 
52 
 
%c Local version of date and time Mon Dec 
31 17:41:00 
2018 
 
%C Century 20 
 
 
 
What is OOP?
OOP stands for Object-Oriented Programming. 
Python is an object-oriented language, allowing you to structure your 
code using classes and objects for better organization and reusability. 
 
• Provides a clear structure to programs 
• Makes code easier to maintain, reuse, and debug 
• Helps keep your code DRY (Don't Repeat Yourself) 
%x Local version of date 12/31/18 
 
%X Local version of time 17:41:00 
 
%% A % character % 
 
%G ISO 8601 year 2018 
 
• Allows you to build reusable applications with less code 
• 
• Classes and objects are the two core concepts in object-oriented 
programming. 
• A class defines what an object should look like, and an object is 
created based on that class. For example: 
Class Objects 
Fruit Apple, Banana, Mango 
Car Volvo, Audi, Toyota 
Create a Class 
To create a class, use the keyword class: 
Example  
Create a class named MyClass, with a property named x: 
class MyClass: 
  x = 5 
Create Object 
Now we can use the class named MyClass to create objects: 
Example 
Create an object named p1, and print the value of x: 
p1 = MyClass() 
print(p1.x) 
Delete Objects 
You can delete objects by using the del keyword: 
Example 
Delete the p1 object: 
del p1 
Multiple Objects 
You can create multiple objects from the same class: 
Example 
Create three objects from the MyClass class: 
p1 = MyClass() 
p2 = MyClass() 
p3 = MyClass() 
 
print(p1.x) 
print(p2.x) 
print(p3.x) 
The pass Statement 
class definitions cannot be empty, but if you for some reason have 
a class definition with no content, put in the pass statement to avoid 
getting an error. 
Example 
class Person: 
  pass 
The self Parameter 
The self parameter is a reference to the current instance of the class. 
It is used to access properties and methods that belong to the class. 
Example  
Use self to access class properties: 
class Person: 
  def __init__(self, name, age): 
    self.name = name 
    self.age = age 
 
  def greet(self): 
    print("Hello, my name is " + self.name) 
 
p1 = Person("Emil", 25) 
p1.greet() 
Note: The self parameter must be the first parameter of any method in 
the class. 
Without self, Python would not know which object's properties you want 
to access: 
Example 
The self parameter links the method to the specific object: 
class Person: 
  def __init__(self, name): 
    self.name = name 
 
  def printname(self): 
    print(self.name) 
 
p1 = Person("Tobias") 
p2 = Person("Linus") 
 
p1.printname() 
p2.printname() 
All classes have a built-in method called __init__(), which is always 
executed when the class is being initiated. 
The __init__() method is used to assign values to object properties, or to 
perform operations that are necessary when the object is being created. 
Example  
Create a class named Person, use the __init__() method to assign values 
for name and age: 
class Person: 
  def __init__(self, name, age): 
    self.name = name 
    self.age = age 
 
p1 = Person("Emil", 36) 
 
print(p1.name) 
print(p1.age) 
 
Note: The __init__() method is called automatically every time the class 
is being used to create a new object. 
 
Without the __init__() method, you would need to set properties 
manually for each object: 
Example 
Create a class without __init__(): 
class Person: 
  pass 
 
p1 = Person() 
p1.name = "Tobias" 
p1.age = 25 
 
print(p1.name) 
print(p1.age) 
Using __init__() makes it easier to create objects with initial values: 
Example 
With __init__(), you can set initial values when creating the object: 
class Person: 
  def __init__(self, name, age): 
    self.name = name 
    self.age = age 
 
p1 = Person("Linus", 28) 
 
print(p1.name) 
print(p1.age) 
 
You can also set default values for parameters in the __init__() method: 
Example 
Set a default value for the age parameter: 
class Person: 
  def __init__(self, name, age=18): 
    self.name = name 
    self.age = age 
 
p1 = Person("Emil") 
p2 = Person("Tobias", 25) 
 
print(p1.name, p1.age) 
print(p2.name, p2.age) 
Multiple Parameters 
The __init__() method can have as many parameters as you need: 
Example 
Create a Person class with multiple parameters: 
class Person: 
  def __init__(self, name, age, city, country): 
    self.name = name 
    self.age = age 
    self.city = city 
    self.country = country 
 
p1 = Person("Linus", 30, "Oslo", "Norway") 
 
print(p1.name) 
print(p1.age) 
print(p1.city) 
print(p1.country) 
Class Properties
Properties are variables that belong to a class. They store data for each 
object created from the class. 
Example  
Create a class with properties: 
class Person: 
  def __init__(self, name, age): 
    self.name = name 
    self.age = age 
 
p1 = Person("Emil", 36) 
 
print(p1.name) 
print(p1.age) 
Access Properties
You can access object properties using dot notation: 
Example 
Access the properties of an object: 
class Car: 
  def __init__(self, brand, model): 
    self.brand = brand 
    self.model = model 
 
car1 = Car("Toyota", "Corolla") 
 
print(car1.brand) 
print(car1.model) 
Modify Properties 
You can modify the value of properties on objects: 
Example 
Change the age property: 
class Person: 
  def __init__(self, name, age): 
    self.name = name 
    self.age = age 
 
p1 = Person("Tobias", 25) 
print(p1.age) 
 
p1.age = 26 
print(p1.age) 
Add New Properties 
You can add new properties to existing objects: 
Example 
Add a new property to an object: 
class Person: 
  def __init__(self, name): 
    self.name = name 
 
p1 = Person("Tobias") 
 
p1.age = 25 
p1.city = "Oslo" 
 
print(p1.name) 
print(p1.age) 
print(p1.city) 
 
                   Class Methods 
Methods are functions that belong to a class. They define the behavior of 
objects created from the class. 
Example  
Create a method in a class: 
class Person: 
  def __init__(self, name): 
    self.name = name 
 
  def greet(self): 
    print("Hello, my name is " + self.name) 
 
p1 = Person("Emil") 
p1.greet() 
 
Note: All methods must have self as the first parameter. 
Methods with Parameters 
Methods can accept parameters just like regular functions: 
Example 
Create a method with parameters: 
class Calculator: 
  def add(self, a, b): 
    return a + b 
 
  def multiply(self, a, b): 
    return a * b 
 
calc = Calculator() 
print(calc.add(5, 3)) 
print(calc.multiply(4, 7)) 
Methods Accessing Properties 
Methods can access and modify object properties using self: 
Example 
A method that accesses object properties: 
class Person: 
  def __init__(self, name, age): 
    self.name = name 
    self.age = age 
 
  def get_info(self): 
    return f"{self.name} is {self.age} years old" 
p1 = Person("Tobias", 28) 
print(p1.get_info()) 
 
 
Inheritance allows us to define a class that inherits all the methods and 
properties from another class. 
Parent class is the class being inherited from, also called base class. 
Child class is the class that inherits from another class, also called 
derived class. 
 
 
 
 
Python Inheritance 
 
 
 
 
 
 
Types of Inheritance: 
1. Single Inheritance: A child class inherits from a single parent class. 
2. Multiple Inheritance: A child class inherits from more than one 
parent class. 
3. Multilevel Inheritance: A child class inherits from a parent class, 
which in turn inherits from another class. 
4. Hierarchical Inheritance: Multiple child classes inherit from a 
single parent class. 
5. Hybrid Inheritance: A combination of two or more types of 
inheritance. 
 
 
Create a Parent Class 
Any class can be a parent class, so the syntax is the same as creating any 
other class: 
Example  
Create a class named Person, with firstname and lastname properties, and 
a printname method: 
class Person: 
  def __init__(self, fname, lname): 
    self.firstname = fname 
    self.lastname = lname 
 
  def printname(self): 
    print(self.firstname, self.lastname) 
 
#Use the Person class to create an object, and then execute the 
printname method: 
 
x = Person("John", "Doe") 
x.printname() 
 
Create a Child Class 
To create a class that inherits the functionality from another class, send 
the parent class as a parameter when creating the child class: 
Example 
Create a class named Student, which will inherit the properties and 
methods from the Person class: 
class Student(Person): 
  pass 
 
Note: Use the pass keyword when you do not want to add any other properties or 
methods to the class. 
Add Properties 
Example 
Add a property called graduationyear to the Student class: 
class Student(Person): 
  def __init__(self, fname, lname): 
    super().__init__(fname, lname) 
    self.graduationyear = 2019 
Example 
Add a year parameter, and pass the correct year when creating objects: 
class Student(Person): 
  def __init__(self, fname, lname, year): 
    super().__init__(fname, lname) 
    self.graduationyear = year 
 
x = Student("Mike", "Olsen", 2019) 
 
 
 
 
 
Inheritance Class Polymorphism 
What about classes with child classes with the same name? Can we use 
polymorphism there? 
Yes. If we use the example above and make a parent class called Vehicle, 
and make Car, Boat, Plane child classes of Vehicle, the child classes inherits 
the Vehicle methods, but can override them: 
Example 
Create a class called Vehicle and make Car, Boat, Plane child classes 
of Vehicle: 
class Vehicle: 
  def __init__(self, brand, model): 
    self.brand = brand 
    self.model = model 
 
  def move(self): 
    print("Move!") 
 
class Car(Vehicle): 
  pass 
 
class Boat(Vehicle): 
  def move(self): 
    print("Sail!") 
 
class Plane(Vehicle): 
  def move(self): 
    print("Fly!") 
 
car1 = Car("Ford", "Mustang")       #Create a Car object 
boat1 = Boat("Ibiza", "Touring 20") #Create a Boat object 
plane1 = Plane("Boeing", "747")     #Create a Plane object 
 
for x in (car1, boat1, plane1): 
  print(x.brand) 
  print(x.model) 
  x.move() 
Class Polymorphism 
Polymorphism is often used in Class methods, where we can have 
multiple classes with the same method name. 
For example, say we have three classes: Car, Boat, and Plane, and they all 
have a method called move(): 
Example 
Different classes with the same method: 
class Car: 
  def __init__(self, brand, model): 
    self.brand = brand 
    self.model = model 
 
  def move(self): 
    print("Drive!") 
 
class Boat: 
  def __init__(self, brand, model): 
    self.brand = brand 
    self.model = model 
 
  def move(self): 
    print("Sail!") 
 
class Plane: 
  def __init__(self, brand, model): 
    self.brand = brand 
    self.model = model 
 
  def move(self): 
    print("Fly!") 
 
car1 = Car("Ford", "Mustang")       #Create a Car object 
boat1 = Boat("Ibiza", "Touring 20") #Create a Boat object 
plane1 = Plane("Boeing", "747")     #Create a Plane object 
 
for x in (car1, boat1, plane1): 
  x.move() 
Python Encapsulation 
Encapsulation is about protecting data inside a class. 
It means keeping data (properties) and methods together in a class, 
while controlling how the data can be accessed from outside the class. 
This prevents accidental changes to your data and hides the internal 
details of how your class works. 
 
Private Properties 
In Python, you can make properties private by using a double 
underscore __ prefix: 
Example  
Create a private class property named __age: 
class Person: 
  def __init__(self, name, age): 
    self.name = name 
    self.__age = age # Private property 
 
p1 = Person("Emil", 25) 
print(p1.name) 
print(p1.__age) # This will cause an error 
Get Private Property Value 
To access a private property, you can create a getter method: 
Example 
Use a getter method to access a private property: 
class Person: 
  def __init__(self, name, age): 
    self.name = name 
    self.__age = age 
 
  def get_age(self): 
    return self.__age 
 
p1 = Person("Tobias", 25) 
print(p1.get_age()) 
 Set Private Property Value 
To modify a private property, you can create a setter method.The setter 
method can also validate the value before setting it: 
Example 
Use a setter method to change a private property: 
class Person: 
  def __init__(self, name, age): 
    self.name = name 
    self.__age = age 
 
  def get_age(self): 
    return self.__age 
 
  def set_age(self, age): 
    if age > 0: 
      self.__age = age 
    else: 
      print("Age must be positive") 
 
p1 = Person("Tobias", 25) 
print(p1.get_age()) 
 
p1.set_age(26) 
print(p1.get_age()) 
 
 
Encapsulation provides several benefits: 
• Data Protection: Prevents accidental modification of data 
• Validation: You can validate data before setting it 
• Flexibility: Internal implementation can change without affecting external 
code 
• Control: You have full control over how data is accessed and modified 
Example 
Use encapsulation to protect and validate data: 
Why Use Encapsulation? 
class Student: 
  def __init__(self, name): 
    self.name = name 
    self.__grade = 0 
 
  def set_grade(self, grade): 
    if 0 <= grade <= 100: 
      self.__grade = grade 
    else: 
      print("Grade must be between 0 and 100") 
 
  def get_grade(self): 
    return self.__grade 
 
  def get_status(self): 
    if self.__grade >= 60: 
      return "Passed" 
    else: 
      return "Failed" 
 
student = Student("Emil") 
student.set_grade(85) 
print(student.get_grade()) 
print(student.get_status()) 
 
Note: A single underscore _ is just a convention. It tells other programmers that the 
property is intended for internal use, but Python doesn't enforce this restriction. 
 
 
 
An inner class is a class defined inside another class. The inner class can 
access the properties and methods of the outer class. 
Inner classes are useful for grouping classes that are only used in one 
place, making your code more organized. 
Example  
Python Inner Classes 
Create an inner class: 
class Outer: 
  def __init__(self): 
    self.name = "Outer Class" 
 
  class Inner: 
    def __init__(self): 
      self.name = "Inner Class" 
 
    def display(self): 
      print("This is the inner class") 
 
outer = Outer() 
print(outer.name) 
 
To access the inner class, create an object of the outer class, and then 
create an object of the inner class: 
Example 
Access the inner class and create an object: 
class Outer: 
  def __init__(self): 
    self.name = "Outer" 
 
  class Inner: 
    def __init__(self): 
      self.name = "Inner" 
 
    def display(self): 
      print("Hello from inner class") 
 
outer = Outer() 
inner = outer.Inner() 
inner.display() 
Accessing Inner Class from The Outside 
Accessing Outer Class from Inner 
Class 
Inner classes in Python do not automatically have access to the outer 
class instance. 
If you want the inner class to access the outer class, you need to pass the 
outer class instance as a parameter: 
Example 
Pass the outer class instance to the inner class: 
class Outer: 
  def __init__(self): 
    self.name = "Emil" 
 
  class Inner: 
    def __init__(self, outer): 
      self.outer = outer 
 
    def display(self): 
      print(f"Outer class name: {self.outer.name}") 
 
outer = Outer() 
inner = outer.Inner(outer) 
inner.display() 
 
 
A class can have multiple inner classes: 
Example 
Create multiple inner classes: 
Multiple Inner Classes 
class Computer: 
  def __init__(self): 
    self.cpu = self.CPU() 
    self.ram = self.RAM() 
 
  class CPU: 
    def process(self): 
      print("Processing data...") 
 
  class RAM: 
    def store(self): 
      print("Storing data...") 
 
computer = Computer() 
computer.cpu.process() 
computer.ram.store() 
Abstraction hides the internal implementation details while exposing only the necessary 
functionality. It helps focus on "what to do" rather than "how to do it." 
Types of Abstraction: 
• Partial Abstraction: Abstract class contains both abstract and concrete methods. 
• Full Abstraction: Abstract class contains only abstract methods (like interfaces). 
Example: In this example, we create an abstract Dog class with an abstract method 
(sound) and a concrete method. Subclasses implement the abstract method while 
inheriting the concrete method. 
 
from abc import ABC, abstractmethod 
class Dog(ABC):  # Abstract Class 
    def __init__(self, name): 
        self.name = name 
    @abstractmethod 
    def sound(self):  # Abstract Method 
        pass 
    def display_name(self):  # Concrete Method 
        print(f"Dog's Name: {self.name}") 
class Labrador(Dog):  # Partial Abstraction 
    def sound(self): 
        print("Labrador Woof!") 
class Beagle(Dog):  # Partial Abstraction 
    def sound(self): 
        print("Beagle Bark!") 
# Example Usage 
dogs = [Labrador("Buddy"), Beagle("Charlie")] 
for dog in dogs: 
    dog.display_name()  # Calls concrete method 
    dog.sound()  # Calls implemented abstract method 
 
Explanation: 
• Partial Abstraction: The Dog class has both abstract (sound) and concrete 
(display_name) methods. 
• Why Use It: Abstraction ensures consistency in derived classes by enforcing the 
implementation of abstract methods. 
 
