# Sheesh Programming Language

## Overview

**Sheesh** is a dynamically-typed interpreted programming language designed for simplicity and ease of use. It supports basic data types such as numbers, strings, and lists, as well as control flow constructs like conditionals (`AGAR` statements), loops (`ISS` and `JABTAK` loops), and function definitions.

## Usage
Download the source and extract it, open the folder in terminal and run `python shell.py`
- You can run the code directly on shell
- Use `RUN(filename)` to run a external file having extension .sheesh.

## Data Types

### Number

- Basic numerical data type.
  ```
  YE num = 2000
  YE dec = 7.8
  ```

### String

- Represents sequences of characters.
```
YE str = "Sheesh"
```
### List

- Represents an ordered collection of values.
```
YE arr = [1,2,3,4,5]
```

## Variables

- Variables are used to store and manage data.
```
YE var1 = 78
YE str1 = "Sheesh"
```

## Operators

### Arithmetic Operators

- `+` (Addition)
- `-` (Subtraction)
- `*` (Multiplication)
- `/` (Division)
- `**` (Exponentiation)

### Comparison Operators

- `==` (Equal to)
- `!=` (Not equal to)
- `<` (Less than)
- `>` (Greater than)
- `<=` (Less than or equal to)
- `>=` (Greater than or equal to)

### Logical Operators

- `AUR` (Logical AND)
- `YA` (Logical OR)
- `NA` (Logical NOT)

## Control Flow

### Conditional Statements
  - `AGAR` (IF)
  - `NAHITOH` (ELSEIF)
  - `WARNA` (ELSE)
  - `TOH` (THEN)
```
YE val = INPUT_INT()
AGAR val == 0 TOH
  PRINT("Number is 0")
NAHITOH val % 2 == 0 TOH
  PRINT("Number is even!")
WARNA val
  PRINT("Number is odd!")
```
### Loops

#### For Loop
```
ISS i = 0 SE 10 TOH
  PRINT(i)
```
#### While Loop
```
YE val = 10

JABTAK val > 0
  val = val - 1
```
### Functions

- Functions are defined using `FUN` keyword.
```
FUN foobar(str)
  AGAR str == "foo"
    WAPAS "bar"
  WARNA
    WAPAS "foo"

foobar("foo") # Will return bar
```  

### Built-in Functions

- `PRINT`, `INPUT`, `LEN`, `APPEND`, `POP`, `EXTEND`, and more.

## Special Keywords

- `NULL`: Represents a null or undefined value.
- `TRUE` and `FALSE`: Boolean values.
- `MATH_PI`: Represents the mathematical constant Pi.

## Built-in Functions

### `PRINT(value)`

Prints the given value to the console.


### `PRINT_RET(value)`

Prints the given value to the console and returns it.


### `INPUT()`

Reads a line of input from the user and returns it as a string.


### `INPUT_INT()`

Reads a line of input from the user and converts it to an integer.


### `CLEAR()`

Clears the console screen.


### `IS_NUM(value)`

Returns `TRUE` if the given value is a number, `FALSE` otherwise.


### `IS_STR(value)`

Returns `TRUE` if the given value is a string, `FALSE` otherwise.


### `IS_LIST(value)`

Returns `TRUE` if the given value is a list, `FALSE` otherwise.


### `IS_FUN(value)`

Returns `TRUE` if the given value is a function, `FALSE` otherwise.


### `APPEND(list, value)`

Adds the specified value to the end of the given list.


### `POP(list, index)`

Removes and returns the element at the specified index from the list.


### `EXTEND(list1, list2)`

Appends all elements from `list2` to the end of `list1`.


### `LEN(list)`

Returns the length of the given list.


### `RUN(filename)`

Executes the Sheesh script in the specified file.



## Example Sheesh Script

- Replace image here with a code displaying an example Sheesh script.
```
# This is a very useful piece of software

FUN oopify(prefix) -> prefix + "oop"

FUN join(elements, separator)
	YE result = "" 

	ISS i = 0 SE LEN(elements) TOH
		YE result = result + elements/i
		AGAR i != LEN(elements) - 1 TOH YE result = result + separator
	KHATAM

	WAPAS result
KHATAM

FUN map(elements, func)
	YE new_elements = []

	ISS i = 0 SE LEN(elements) TOH
		APPEND(new_elements, func(elements/i))
	KHATAM

	WAPAS new_elements
KHATAM

PRINT("Greetings universe!")

ISS i = 0 SE 5 TOH
	PRINT(join(map(["l", "sp"], oopify), ", "))
KHATAM
```
This documentation provides a high-level overview of the Sheesh programming language. For more detailed information, including error handling, advanced features, and additional examples, please contact at `shhhshank@gmail.com`.
