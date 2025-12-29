
### 1. Python Basics
• Variables, Data types  
• Input/Output  
• Operators  
• Conditional statements (if-else)  
• Loops (for, while)

### 2. Data Structures
• Lists, Tuples, Sets, Dictionaries  
• List/Dict Comprehensions

### 3. Functions & Modules 
• Defining & calling functions  
• Arguments, return values  
• `import` & creating modules

### 4. File Handling  
• Read/write text & CSV files  
• Use of `with open()`

### 5. Object-Oriented Programming
• Classes & Objects  
• Inheritance, Polymorphism  
• Constructors (`_init_`)  

### 6. Error Handling
• try-except blocks  
• finally, raise

### 7. Useful Built-in Modules
• `math`, `datetime`, `random`, `os`

### 8. Libraries for Practice
• NumPy & Pandas (Data handling)  
• Matplotlib & Seaborn (Visualization)


#### 1. What is Python?
Python is a beginner-friendly, high-level programming language used for web development, data science, automation, AI, and more.  

```python
print("Hello, World!")
```

#### 2. Variables*  
Used to store data in memory that can be used later.  

```python
name = "Alice"
age = 25
```

#### 3. Data Types 
Python supports various built-in types like integers, strings, floats, booleans, lists, and dictionaries.  
``` 
x = 10          # int  
pi = 3.14       # float  
text = "Hi"     # string  
is_valid = True # bool  
colors = ["red", "blue"]        # list  
user = {"name": "Bob", "age": 30}  # dictionary
```

#### 4. Conditional Statements
Used to make decisions based on conditions (`if`, `elif`, `else`).  

```python
if age >= 18:
    print("Adult")
else:
    print("Minor")
```

#### 5. Loops  
Used to repeat a block of code.  

```python
for loop
for i in range(3):
    print(i)

while loop
count = 0
while count < 3:
    print(count)
    count += 1
```

#### 6. Functions 
Reusable blocks of code that perform a task.  

```python
def greet(name):
    return f"Hello, {name}"

print(greet("Sara"))
```

#### 7. Lists
Ordered, mutable collection of items.  

```python
fruits = ["apple", "banana", "cherry"]
print(fruits[1])  # banana
```

#### 8. Dictionaries
Stores data as key-value pairs.  

```python
person = {"name": "John", "age": 30}
print(person["name"])
```

#### 9. File Handling 
Used to read/write files.  

```python
with open("data.txt", "r") as file:
    content = file.read()
    print(content)
```

#### 10. Modules & Imports 
Lets you use external code and libraries.  

```python
import math
print(math.sqrt(16))
```

## Python Coding Interview Questions with Answers: 

### 1️. Reverse a String

##### Q: Write code to reverse a given string.  
 
```python
def reverse_string(s):
    return s[::-1]

print(reverse_string("hello"))  # Output: "olleh"
```

### 2️. Check Palindrome 

#### Q: Check if a string is a palindrome (ignoring spaces & case).  

```python
## A palindromic number is a number that remains the same when its digits are reversed.
## This means it has reflectional symmetry across a vertical axis.
## 12321 is palindrom (121,131,141, like...)

def is_palindrome(s):
    s = s.replace(" ", "").lower()
    return s == s[::-1]

print(is_palindrome("Race car"))  # Output: True
```

### 3️. Find Duplicate Elements in List

#### Q: Print all duplicates from a list.  
 
```python
from collections import Counter

def find_duplicates(lst):
    count = Counter(lst)
    return [item for item, freq in count.items() if freq > 1]

print(find_duplicates([1, 2, 3, 2, 4, 1]))  # Output: [1, 2]
```

### 4️. Count Vowels in a String 

#### Q: Count number of vowels in a string.  

```python
def count_vowels(s):
    return sum(1 for char in s.lower() if char in "aeiou")

print(count_vowels("Python is fun"))  # Output: 4
```

### 5️. Find Factorial Using Recursion

#### Q: Write a recursive function to find factorial. 
 
```python
def factorial(n):
    if n == 0 or n == 1:
        return 1
    return n * factorial(n - 1)

print(factorial(5))  
# Output: 120
```

### 6️. Find the Largest Element in a List 

#### Q: Return the largest number in a list.  
```python
def find_max(lst):
    return max(lst)

print(find_max([3, 7, 2, 9, 5]))  # Output: 9
```

### 7️. Check for Anagrams 

#### Q: Check if two strings are anagrams.  
```python
def are_anagrams(s1, s2):
    return sorted(s1.lower()) == sorted(s2.lower())

print(are_anagrams("listen", "silent"))  # Output: True
```

### 8️. Remove Punctuation from String 

#### Q: Clean a string by removing all punctuation.  
```python
import string

def remove_punctuation(s):
    return ''.join(c for c in s if c not in string.punctuation)

print(remove_punctuation("Hello, World!"))  # Output: Hello World
```

### 9️. Fibonacci Using Recursion

#### Q: Generate nth Fibonacci number.  
```python
def fibonacci(n):
    if n <= 1:
        return n
    return fibonacci(n-1) + fibonacci(n-2)

print(fibonacci(6))  # Output: 8
```

### 10. Flatten a Nested List

#### Q: Flatten a list of lists into a single list.  
```python
def flatten(lst):
    return [item for sublist in lst for item in sublist]

print(flatten([[1, 2], [3, 4], [5]]))  # Output: [1, 2, 3, 4, 5]

        or

def rec_lst(lst):
    res=[]
    for sublist in lst:
        for item in sublist:
            res.append(item)
    return res
rec_lst([[1, 2], [3, 4], [5]])
```


### 11. Remove Duplicates from a List

#### Q: Remove duplicates while preserving the original order.
```python
def remove_duplicates(lst):
    seen = set()
    return [x for x in lst if not (x in seen or seen.add(x))]

print(remove_duplicates([1, 2, 2, 3, 1, 4]))  # Output: [1, 2, 3, 4]

            or

def rem_dup(lst):
    seen =set()
    result = []
    for item in lst:
        if item not in seen:
            seen.add(item)
            result.append(item)
    return result
rem_dup([1,2,3,4,5,3,4,1])

# lst = [1,2,3,4,5,3,4,1]
# seen = set() -- create an empty set to track seen elements
# result = [] -- create an empty list to store unique elements
# for item in lst:
# if item not in seen
# we add item to seen set and append it to result list
# seen.add(item)
# we append item to result list
# result.append(item)

```

### 12. Merge Two Dictionaries

#### Q: Merge two dictionaries into one.
```python
def merge_dicts(d1, d2):
    return {**d1, **d2} // unpacking with multiple dictionaries

print(merge_dicts({'a': 1}, {'b': 2}))  # Output: {'a': 1, 'b': 2}
```

### 13. Find the Most Frequent Element

#### Q: Find the element that appears most frequently in a list.
```python
from collections import Counter

def most_frequent(lst):
    return Counter(lst).most_common(1)[0][0]

print(most_frequent([1, 3, 1, 3, 2, 1]))  # Output: 1
```

### 14. Check for Prime Number

#### Q: Determine if a number is prime.
```python
def is_prime(n):
    if n <= 1:
        return False
    for i in range(2, int(n**0.5)+1):
        if n % i == 0:
            return False
    return True

print(is_prime(7))  # Output: True
```

### 15. Find All Even Numbers in a List

#### Q: Return all even numbers from a list.
```python
def find_evens(lst):
    return [x for x in lst if x % 2 == 0]

print(find_evens([1, 2, 3, 4, 5, 6]))  # Output: [2, 4, 6]
```

### 16. Sum of Digits of a Number
#### Q: Write a function to return the sum of digits of a number.
```python
def sum_of_digits(n):
    return sum(int(digit) for digit in str(abs(n)))

print(sum_of_digits(1234))  # Output: 10
```

### 17. Check if List is Sorted
#### Q: Determine if a list is sorted in ascending order.
```python
def is_sorted(lst):
    return lst == sorted(lst)

print(is_sorted([1, 2, 3, 4]))  # Output: True
print(is_sorted([3, 2, 1]))    # Output: False
```

### 18. Count Words in a String
#### Q: Count the number of words in a string.
```python
def count_words(s):
    return len(s.split())

print(count_words("Python is awesome"))  # Output: 3
```

### 19. Find Common Elements Between Two Lists
#### Q: Return common elements from two lists.
```python
def common_elements(lst1, lst2):
    return list(set(lst1) & set(lst2))

print(common_elements([1, 2, 3], [2, 3, 4]))  # Output: [2, 3]
```

### 20. Convert String to Title Case
#### Q: Convert a string to title case (capitalize each word).
```python
def to_title_case(s):
    return s.title()

print(to_title_case("python is fun"))  # Output: Python Is Fun
```

#### 21. Find Missing Number in a List  
##### Q: Find the missing number from 1 to n.  
```python
def find_missing(nums, n):  
    return n * (n + 1) // 2 - sum(nums)

print(find_missing([1, 2, 4, 5], 5))  # Output: 3
```

#### 22. Swap Two Variables Without Temp  
##### Q: Swap two numbers without using a third variable.  
```python
a, b = 5, 10  
a, b = b, a  
print(a, b)  # Output: 10 5
```

#### 23. Count Character Frequency  
##### Q: Count frequency of each character in a string.  
```python
from collections import Counter

def char_frequency(s):  
    return Counter(s)

print(char_frequency("python"))
```

#### 24. Check Armstrong Number  
##### Q: Check if a number is an Armstrong number.  
```python
def is_armstrong(n):  
    digits = [int(d) for d in str(n)]  
    return n == sum(d**len(digits) for d in digits)

print(is_armstrong(153))  # Output: True
```

#### 25. Reverse Words in a Sentence  
##### Q: Reverse words while keeping order.  
```python
def reverse_words(s):  
    return " ".join(word[::-1] for word in s.split())

print(reverse_words("Python is fun"))  
Output: nohtyP si nuf
```

#### 26. Check if Two Lists Are Equal 
##### Q: Check whether two lists contain the same elements in the same order.  
```python
def lists_equal(l1, l2):
    return l1 == l2

print(lists_equal([1, 2, 3], [1, 2, 3]))  # True  
print(lists_equal([1, 2, 3], [3, 2, 1]))  # False
```

#### 27. Find Intersection of Two Lists  
##### Q: Return common elements without duplicates.  
```python
def intersection(l1, l2):
    return list(set(l1) & set(l2))

print(intersection([1, 2, 3, 4], [3, 4, 5]))  # [3, 4]
```

#### 28. Check Leap Year
##### Q: Check whether a year is a leap year.  
```python
def is_leap(year):
    return year % 400 == 0 or (year % 4 == 0 and year % 100 != 0)

print(is_leap(2024))  # True
```

#### 29. Count Occurrences of an Element
##### Q: Count how many times an element appears in a list.  
```python
def count_occurrences(lst, x):
    return lst.count(x)

print(count_occurrences([1, 2, 2, 3, 2], 2))  # 3
```

#### 30. Check if String Contains Only Digits  
##### Q: Verify whether a string has digits only.  
```python
def is_digits(s):
    return s.isdigit()

print(is_digits("12345"))  # True  
print(is_digits("123a"))   # False
```

#### 31. Find the Second Largest Number  
##### Q: Return the second largest element in a list.  
```python
def second_largest(lst):
    return sorted(set(lst))[-2]

print(second_largest([10, 20, 4, 45, 99]))  # Output: 45
```

#### 32. Check if String Has All Unique Characters 
##### Q: Verify all characters are unique.  
```python
def has_unique_chars(s):
    return len(s) == len(set(s))

print(has_unique_chars("python"))  # Output: True  
print(has_unique_chars("hello"))   # Output: False
```

#### 33. Find GCD of Two Numbers
##### Q: Compute the greatest common divisor.  
```python
import math

def gcd(a, b):
    return math.gcd(a, b)

print(gcd(20, 28))  # Output: 4
```

#### 34. Count Uppercase and Lowercase Letters
##### Q: Count uppercase and lowercase characters in a string.  
```python
def count_case(s):
    upper = sum(1 for c in s if c.isupper())
    lower = sum(1 for c in s if c.islower())
    return upper, lower

print(count_case("PyThOn"))  # Output: (3, 3)
```

#### 35. Find Longest Word in a Sentence
##### Q: Return the longest word from a sentence.  
```python
def longest_word(s):
    words = s.split()
    return max(words, key=len)

print(longest_word("Python coding interviews are easy"))  
Output: interviews
```

### 36. Check if Number Is Power of Two
#### Q: Determine whether a number is a power of two.  
```python
def is_power_of_two(n):
    return n > 0 and (n & (n - 1)) == 0

print(is_power_of_two(16))  # True
print(is_power_of_two(18))  # False
```

### 37. Remove All Whitespaces from String
#### Q: Remove spaces, tabs, and newlines from a string.  
```python
def remove_spaces(s):
    return "".join(s.split())

print(remove_spaces("Py th on \n"))  # Python
```

### 38. Find First Non-Repeating Character 
#### Q: Return the first character that does not repeat.  
```python
from collections import Counter

def first_unique(s):
    freq = Counter(s)
    for c in s:
        if freq[c] == 1:
            return c
    return None

print(first_unique("swiss"))  # w
```

### 39. Rotate List by k Positions  
#### Q: Rotate a list to the right by k steps.  
```python
def rotate_list(lst, k):
    k %= len(lst)
    return lst[-k:] + lst[:-k]

print(rotate_list([1, 2, 3, 4, 5], 2))  # [4, 5, 1, 2, 3]
```

### 40. Check Balanced Parentheses
#### Q: Check whether parentheses are balanced.  
```python
def is_balanced(s):
    stack = []
    pairs = {')': '(', ']': '[', '}': '{'}
    for c in s:
        if c in pairs.values():
            stack.append(c)
        elif c in pairs:
            if not stack or stack.pop() != pairs[c]:
                return False
    return not stack

print(is_balanced("({[]})"))  # True
print(is_balanced("({[})"))   # False
```


