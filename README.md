# 🌟 Python String Mastery 🌟

There are many data types in Python which among all of them, **string** data type is one of the most used so knowing it well is really important. It's fun to say that one thing you should have encountered in programming so far, is the most basic program: print("Hello, World!"), which simply prints a string to the terminal. Everything started from a string... 

In this document we will be disscussing the most usefull info about string data type. 

<p align="center">
<img width="50%" src="media/213911110-aedbef38-a29f-4b6b-a65c-11608b4f75a5.gif">
</p>

<img width="100%" src="media/212284100-561aa473-3905-4a80-b561-0d28506553ee.gif">

**Table of content:** ☕

1. [What is a string?](#what-is-a-string)
    - [Escape sequences and It's coresponding charachters](#escape-sequences-and-its-coresponding-charachters)

2. [String indexing and slicing](#string-indexing-and-slicing)

3. [String operators](#string-operators)
    - [Arithmetic operators](#arithmetic-operators)
    - [Membership operators](#membership-operators)

4. [Built-in str class and built-in functions](#built-in-str-class-and-built-in-functions)

5. [Built-in String Functions](#built-in-string-functions)
    - [ord()](#ordcharacter)
    - [chr()](#chrnumber)
    - [len()](#lenstring)
    - [str()](#strobject)

6. [Built-in str class Methods](#built-in-str-class-methods)
    - [Case Conversion methods](#case-conversion-methods)
    - [Find and Replace methods](#find-and-replace-methods)
    - [Character Classification methods](#character-classification-methods)
    - [String Formatting methods](#string-formatting-methods)
    - [Methods for converting Between Strings and Lists](#methods-for-converting-between-strings-and-lists)

7. [Modify strings](#modify-strings)

8. [Resources](#resources)

<img width="100%" src="media/212284100-561aa473-3905-4a80-b561-0d28506553ee.gif">

<img width="100%" src="media/212750996-938b257b-266c-45a7-9af7-655341c0f58b.gif">

## What is a string?

***Strings*** are a data type in python which contain characters. The type of a string is `str`, and it can contain any type of characters. Strings are an immutable data type and they can not be changed after they are created. String literals can be enclosed by either double `"` or single `'` quotes. Character escaping is also allowed in strings using the backslash `\`.

---
### Escape sequences and It's coresponding charachters

Escape sequences are used within string using a backslash `\`. You can see some of the most used escapes in the table below.

| Escape Sequence | Character |
| --------------- | --------- |
| \t | Tab |
| \n | Newline |
| \r | Carriage Return |
| \r\n | Carriage Return + Line Feed |
| \v | Line tabulation |


**Example:**

```bash
string = 'Hello,\t\tworld!'
print(string)

# Output
Hello,          world!
```

<img width="100%" src="media/212284100-561aa473-3905-4a80-b561-0d28506553ee.gif">

## String indexing and slicing

**String indexing:** Often in programming languages, individual items in an ordered set of data can be accessed directly using a numeric index or key value. This process is referred to as indexing. In Python, **strings** are ordered sequences of character data, and thus can be indexed in this way. ***Individual*** characters in a string can be accessed by specifying the string name followed by a number in square brackets (`[]`). 

> [!NOTE]
> String indexing in Python is zero-based: the first character in the string has index 0, the next has index 1, and so on. The index of the last character will be the length of the string minus one.

**Example:**

```bash
string = 'Hello'
-------------------------
length = 5
first character index = 0
last character index = 4
```

<img width="100%" src="media/212284100-561aa473-3905-4a80-b561-0d28506553ee.gif">

## String operators

There are only 2 types of operators that can be used with strings:

1. Arithmetic operators
    - \+ Addition
    - \* Multiplication
2. Membership operators
    - in -> value in string
    - not in -> value not in string

> [!NOTE]
> Out of all the Arithmetic operators, only addition and multiplication can be used with strings.

---
### Arithmetic operators

**Addition:** The \+ operator **concatenates** strings. It returns a string consisting of the operands joined together.

**Multiplication:** The \* operator creates multiple copies of a string. One operand must be a string and the other one an integer. The output will be the original string printed multiple times. **Note that if you use 0 or negative numbers the output will be an empty string.**

---
### Membership operators

**in**: Python also provides a membership operator that can be used with strings. The **in** operator returns True if the first operand is contained within the second, and False otherwise.

**not in**: This is the reverse of **in** operator. 

<img width="100%" src="media/212284100-561aa473-3905-4a80-b561-0d28506553ee.gif">

## Built-in str class and built-in functions

Python has a built-in string class named **"str"** with many handy features (there is an older module named **"string"** which you should not use). In the next parts of this document we will see the methods of the `str` class and their use cases. 

Plus: There are some built in functions in python that can be used with strings which will be mentiond later.

> [!IMPORTANT]
> **Functions** are callable procedures that you can invoke to perform specific tasks. **Methods** are similar to functions. A method is a specialized type of callable procedure that is tightly associated with an object. Like a function, a method is called to perform a distinct task, but it is invoked on a specific object and has knowledge of its target object during execution.

<img width="100%" src="media/212284100-561aa473-3905-4a80-b561-0d28506553ee.gif">

## Built-in String Functions

There are some built-in functions in python that work well with strings.

| Function | Description |
| -------- | ----------- |
| ord(`<character>`) | Converts a character to an integer |
| chr(`<number>`) | Converts an integer to a character |
| len(`<string>`) | Returns the length of a string |
| str(`<object>`) | Returns a string representation of an object |

These functions are explored fully below.

---
### ord(`<character>`)

At the most basic level, computers store all information as numbers. To represent character data, a translation scheme is used which maps each character to its representative number.

To keep things simple: `ord(<character>)` Returns an integer value for the given character.

> [!NOTE]
> `ord()` function will return numeric values for Unicode characters as well. Like: €, ∑

---
### chr(`<number>`)

`chr()` does the reverse of `ord()`. Given a numeric value number, `chr(number)` returns a string representing the **character** that corresponds to **number**.

To keep things simple: `chr(<number>)` Returns a character value for the given integer.

> [!NOTE]
> `chr()` handles Unicode characters as well.

---
### len(`<string>`)

With `len()`, you can check Python string length. **len(string)** returns the number of characters in string.

> [!NOTE]
> `len()` works with other data sequences as well.

---
### str(`<object>`)

Virtually any object in Python can be rendered as a string. **str(object)** returns the string representation of object.

> [!NOTE]
> `str()` works with any type of python objects.

<img width="100%" src="media/212284100-561aa473-3905-4a80-b561-0d28506553ee.gif">

## Built-in str class Methods

As said before methods are invoked on objects. [See here](#built-in-str-class-and-built-in-functions)

The syntax for invoking a method on an object is as follows:

```bash
obj.method(<args>)
```
This invokes method `.method()` on object `obj`. `<args>` specifies the arguments passed to the method (if there is any).

> [!NOTE]
> Our object here is a string.

There are 5 diffrent categories of str class methods that we can use on strings:

1. Case Conversion
2. Find and Replace
3. Character Classification
4. String Formatting
5. Converting Between Strings and Lists

In the next parts, I will be writing about the most used str class, methods.

> [!NOTE]
> We will be using a string object for the following parts. keep in mind that everything in python is an object.

```bash
string_obj = "I love myself so much"
```

---
### Case Conversion methods

Methods in this group perform case conversion on the target string.

- string_obj.capitalize() -> Capitalizes the target string.

- string_obj.lower() -> Converts alphabetic characters to lowercase.

- string_obj.upper() -> Converts alphabetic characters to uppercase.

- string_obj.swapcase() -> Swaps case of alphabetic characters. Upper to lower and lower to upper.

- string_obj.title() -> Converts the target string to “title case.” The first letter of every word is in upper.

---
### Find and Replace methods

These methods provide various means of searching the target string for a specified substring. Each method in this group supports optional `<start>` and `<end>` arguments. **start** and **end** are used for slicing.

- string_obj.count(`<sub-string>`, `<start>`, `<end>`) -> Counts occurrences of a substring in the target string.

- string_obj.startswith(`<prefix>`, `<start>`, `<end>`) -> Determines whether the target string starts with a given substring. Output of this method is boolean.

- string_obj.endswith(`<suffix>`, `<start>`, `<end>`) -> Determines whether the target string ends with a given substring. Output of this method is boolean.

- string_obj.find(`<sub-string>`, `<start>`, `<end>`) -> Searches the target string for a given substring. This method returns **-1** if the specified substring is not found. Else the index of the pattern found in the string will be returned. Keep in mind that if you use **start** and **end** then the search will be limited to the slice.

- string_obj.index(`<sub-string>`, `<start>`, `<end>`) -> Searches the target string for a given substring. This method is identical to .find(), except that it raises an exception if `<sub-string>` is not found rather than returning **-1**.

---
### Character Classification methods

Methods in this group classify a string based on the characters it contains.

- string_obj.isalnum() -> Determines whether the target string consists of alphanumeric characters. 

- string_obj.isalpha() -> Determines whether the target string consists of only alphabetic characters.

- string_obj.isdigit() -> Determines whether the target string consists of only digit characters.

- string_obj.islower() -> Determines whether the target string’s alphabetic characters are all in lowercase.

- string_obj.isupper() -> Determines whether the target string’s alphabetic characters are all in uppercase.

---
### String Formatting methods

Methods in this group modify or enhance the format of a string.

- string_obj.center(`<width>`, `<fill>`) -> Centers a string in a field. Creates padding for the string from both sides equal to **width**. Originaly padding is consisted of white spaces but it can be customized using **fill**.

- string_obj.strip(`<chars>`) -> Strips characters from the left and right ends of a string. If the optional `<chars>` argument is specified, then the set of characters specified will be removed in the result. Please note that this method has `rstrip()` and `lstrip()` versions too.

- string_obj.replace(`<old-substring>`, `<new-substring>`, `<count>`) -> Replaces occurrences of a substring within a string.If the optional `<count>` argument is specified, a maximum of `<count>` replacements are performed, starting at the left end of string.

---
### Methods for converting Between Strings and Lists 

Methods in this group convert between a string and some composite data type by either pasting objects together to make a string, or by breaking a string up into pieces.

These methods operate on or return iterables, the general Python term for a sequential collection of objects.

- "ch".join(`<iterable>`) -> Concatenates strings from an iterable. This returns the string that results from concatenating the objects in `<iterable>` separated by ch.

- string_obj.partition(`<seperator>`) -> Divides a string based on a separator. This splits string_obj at the first occurrence of string `<seperator>`. The return value is a three-part tuple consisting of: 
    - The portion of s preceding `<seperator>`.
    - `<seperator>` itself.
    - The portion of s following `<seperator>`.

- string_obj.split(seperator=None, maxsplit=None) -> Splits a string into a list of substrings. If seperator is not defined then the defalt: **white-space**, will be considered by python. If the optional keyword parameter `<maxsplit>` is specified, a maximum of that many splits are performed.

- string_obj.splitlines() -> Breaks a string at line boundaries. And returns the lines in a list.

<img width="100%" src="media/212284100-561aa473-3905-4a80-b561-0d28506553ee.gif">

## Modify strings

To tell the truce strings cannot be modified. It's because strings are an immutable data type in python, so they cannot be changed. However there is no need to actualy modify strings, this kind of changes can be accomplished by making a new copy of the original string which contain's the changes.

There are many possible ways to do this, but 2 approaches are most used in this case, which are:

1. using string **slicing** combined with string **concatination**.

```bash
string = 'foobar'
new_string = string[:3] + 'x' + string[4:]
print(new_string)

# Output
'fooxar'
```

2. using the built-in str class **`replace()`** method.

```bash
string = 'foobar'
new_string = string.replace('b', 'x')
print(new_string)

# Output
'fooxar'
```

<img width="100%" src="media/212284100-561aa473-3905-4a80-b561-0d28506553ee.gif">

<img width="100%" src="media/212284100-561aa473-3905-4a80-b561-0d28506553ee.gif">

<img width="100%" src="media/212284100-561aa473-3905-4a80-b561-0d28506553ee.gif">


## Resources

- [RealPython: Strings and Character Data in Python](https://realpython.com/python-strings/)

- [Google for Education: python strings](https://developers.google.com/edu/python/strings)

<p align="center">
<img width="50%" src="media/216656956-c5f97119-4de0-4e55-8906-c2699cc43ccd.gif">
</p>