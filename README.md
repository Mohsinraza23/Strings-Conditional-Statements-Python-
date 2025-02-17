# Strings-Conditional-Statements-Python-

# Strings in Python

## Concatenation
String is a data type that stores a sequence of characters.

```python
"hello" + "world" # Output: "helloworld"
```

## Length of a String
```python
len(str)
```

## Indexing
```plaintext
C o d e _ w i t h _ M o h s i n
0 1 2 3 4 5 6 7 8 9 10 11 12 13 14 15
```
```python
str = "Code_with_Mohsin"
print(str[0]) # Output: 'C'
print(str[1]) # Output: 'o'
```

**Note:** Strings are immutable in Python, so `str[0] = 'B'` is not allowed.

---

## Slicing
Syntax:
```python
str[starting_idx : ending_idx] # ending_idx is not included
```
Examples:
```python
str = "CodeWithMohsin"
print(str[1:4])  # Output: "ode"
print(str[:4])   # Output: "Code"
print(str[1:])   # Output: "odeWithMohsin"
```

## Negative Indexing
```plaintext
A p p l e
-5 -4 -3 -2 -1
```
```python
str = "Apple"
print(str[-3:-1]) # Output: "pl"
```

---

## String Functions
```python
str = "I am a coder."
print(str.endswith("er."))  # Output: True
print(str.count("am"))       # Output: 1
print(str.capitalize())       # Output: "I am a coder."
print(str.find("coder"))     # Output: 7
print(str.replace("coder", "developer")) # Output: "I am a developer."
```

---

## Let's Practice
1. **WAP to input user’s first name & print its length.**
   ```python
   name = input("Enter your first name: ")
   print("Length of name:", len(name))
   ```
2. **WAP to find the occurrence of ‘$’ in a String.**
   ```python
   string = input("Enter a string: ")
   print("Occurrences of '$':", string.count('$'))
   ```

---

# Conditional Statements

## if-elif-else (SYNTAX)
```python
if condition:
    statement1
elif condition:
    statement2
else:
    statementN
```

## Example: Grading System
```python
marks = int(input("Enter marks: "))
if marks >= 90:
    grade = "A"
elif marks >= 80:
    grade = "B"
elif marks >= 70:
    grade = "C"
elif marks >= 60:
    grade = "D"
else:
    grade = "F"
print("Your Grade:", grade)
```

---

## Let's Practice
1. **WAP to check if a number entered by the user is odd or even.**
   ```python
   num = int(input("Enter a number: "))
   if num % 2 == 0:
       print("Even Number")
   else:
       print("Odd Number")
   ```

2. **WAP to find the greatest of 3 numbers entered by the user.**
   ```python
   a = int(input("Enter first number: "))
   b = int(input("Enter second number: "))
   c = int(input("Enter third number: "))
   print("Greatest number:", max(a, b, c))
   ```

3. **WAP to check if a number is a multiple of 7 or not.**
   ```python
   num = int(input("Enter a number: "))
   if num % 7 == 0:
       print("Multiple of 7")
   else:
       print("Not a multiple of 7")
