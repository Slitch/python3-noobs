Here are some exercises to help you get used to list comprehensions in Python:
Exercise 1: Simple List Comprehension

Task: Create a list of squares for numbers from 1 to 10 using list comprehension.

Normal loop way:

squares = []
for x in range(1, 11):
    squares.append(x**2)

print(squares)

Comprehension List Way:

squares = [x**2 for x in range(1, 11)]
print(squares)


Exercise 2: Filtering with List Comprehension
Task: Given a list of numbers, create a new list that contains only the even numbers.

Normal loop way:

numbers = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10]
evens = []
for x in numbers:
    if x % 2 == 0:
        evens.append(x)

print(evens)

Comprehension List Way:

numbers = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10]
evens = [x for x in numbers if x % 2 == 0]
print(evens)


Exercise 3: Using a Function in List Comprehension
Task: Given a list of words, create a new list with the lengths of those words.

Normal Loop Way:

words = ["hello", "world", "python", "is", "awesome"]
lengths = []
for word in words:
    lengths.append(len(word))

print(lengths)

Comprehension List Way:

words = ["hello", "world", "python", "is", "awesome"]
lengths = [len(word) for word in words]
print(lengths)

Exercise 4: Conditional Expressions in List Comprehension
Task: Create a list of numbers from 1 to 20, but replace every number divisible by 3 with the string "Fizz".

Normal Loop Way:

fizz_list = []
for x in range(1, 21):
    if x % 3 == 0:
        fizz_list.append("Fizz")
    else:
        fizz_list.append(x)

print(fizz_list)

Comprehension List Way:

fizz_list = ["Fizz" if x % 3 == 0 else x for x in range(1, 21)]
print(fizz_list)


Exercise 5: Nested List Comprehensions
Task: Create a 3x3 matrix using list comprehension.

Normal Loop Way:

matrix = []
for i in range(3):
    row = []
    for j in range(3):
        row.append(0)
    matrix.append(row)

print(matrix)

Comprehension List Way:

matrix = [[j for j in range(3)] for i in range(3)]
print(matrix)


Exercise 6: Flatten a List of Lists
Task: Flatten a given 2D list into a 1D list.

Normal Loop Way:

matrix = [[1, 2, 3], [4, 5, 6], [7, 8, 9]]
flat_list = []
for sublist in matrix:
    for num in sublist:
        flat_list.append(num)

print(flat_list)

Comprehension List Way:

matrix = [[1, 2, 3], [4, 5, 6], [7, 8, 9]]
flat_list = [num for row in matrix for num in row]
print(flat_list)


Exercise 7: List Comprehension with Strings
Task: Given a list of sentences, create a list of words by splitting each sentence into words.

Normal Loop Way:

sentences = ["Hello world", "List comprehensions are powerful", "Practice makes perfect"]
words = []
for sentence in sentences:
    for word in sentence.split():
        words.append(word)

print(words)

Comprehension List Way:

sentences = ["Hello world", "List comprehensions are powerful", "Practice makes perfect"]
words = [word for sentence in sentences for word in sentence.split()]
print(words)


Exercise 8: Convert Celsius to Fahrenheit
Task: Given a list of temperatures in Celsius, create a list of temperatures in Fahrenheit using the formula F=95C+32F=59​C+32.
F=9/3 C + 32

Normal Loop Way:

celsius = [0, 10, 20, 30, 40]
fahrenheit = []
for temp in celsius:
    fahrenheit.append((9/5) * temp + 32)

print(fahrenheit)

Comprehension List Way:

celsius = [0, 10, 20, 30, 40]
fahrenheit = [(9/5) * temp + 32 for temp in celsius]
print(fahrenheit)


Exercise 9: Extract Digits from a String
Task: Given a string, create a list of digits found in the string.

Normal Loop Way:

string = "There are 3 apples and 5 bananas"
digits = []
for char in string:
    if char.isdigit():
        digits.append(char)

print(digits)

Comprehension List Way:

string = "There are 3 apples and 5 bananas"
digits = [char for char in string if char.isdigit()]
print(digits)


Exercise 10: List Comprehension with Dictionaries
Task: Given a dictionary, create a list of keys that have even values.

Normal Loop Way:

my_dict = {'a': 1, 'b': 2, 'c': 3, 'd': 4}
even_keys = []
for key, value in my_dict.items():
    if value % 2 == 0:
        even_keys.append(key)

print(even_keys)


Comprehension List Way:

my_dict = {'a': 1, 'b': 2, 'c': 3, 'd': 4}
even_keys = [key for key, value in my_dict.items() if value % 2 == 0]
print(even_keys)


Try to work through these exercises and get comfortable with using list comprehensions. They are a very useful tool in Python programming.

