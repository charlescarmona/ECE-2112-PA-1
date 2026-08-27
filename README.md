# ECE-2112-PA-1

**Made by : Charles John M. Carmona | 2ECE-B**

The content of this repository contains the Programming Assignment for the course " Advance Computer Programming " this S.Y. 2026-2027.

# **1. WORD ROTATION PROBLEM**

Create a function that takes a string and returns a string with its first character placed at the end of the string.

The following functions and methods were used in this problem:
- `rotate_word()` - A user-defined function

- `text[1:]` - A string slicing method wherein it takes character starting from index 1 through the end of the string.

Example: `rotate_word("python")` >>> ython

`+ text[0]` - A string indexing method wherein it takes the character from index 0. The user can add it now to the `text[1:]`, afterwards it will return the string with its original index 0 at the end of the string.

Exampkle: `rotate_word("python")` >>> ythonp

```python
def rotate_word(text):
  return text[1:] + text[0]

print (rotate_word("pyhton"))
```
#**2. Username Builder Problem**

Create a function that takes two strings and returns the two strings with its letters converted to lowercase and conjoined with a period.

The functions and methods that were used in approaching this problem are:
- `make_username(first_name, last_name)` - a user-defined function that takes two strings and conjoining them, making the strings appear in a username-like format.

Two built-in string methods were used in this problem. The first string method makes the string become lowercase while the second string method removes the spaces of the strings, conjoining both of them.

```python
first_name.lower().replace(" ", "")
last_name.lower().replace(" ", "")
```

This is then returned by combining the first abnd second string through the following code:

```python
return first_name + "." + last_name
```

Through doing all of the code shown above, the final function for this certain problem would be:

```python
def make_username(first_name, last_name):
  first_name = first_name.lower().replace(" ", "")
