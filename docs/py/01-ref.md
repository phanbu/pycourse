# Expression Types
| Type | Example |
| ---- | ------- |
| Integer | 4,  0,  or  -12 |
| Floating Point | 4.0,  0.0,  or  -12.0 |
| Boolean | True  or  False |
| Complex | not used in this course |

| Type | Description | Example |
| ---- | ----------- | ------- |
| String	| Immutable ordered sequence of characters, uses quote or double quote or block quotes | 'string'  or  "string"  or '''string'''  or  """string""" |
| List | Mutable ordered sequence, always in brackets | [1 , 2, 'three', 4] |
| Tuple	| Immutable ordered sequence, always in parentheses | (a, b, c) |
| Set |	Unordered collection with no duplicates, uses curly braces | { 1, 3, 6 } |
| Dictionary	| Key value pairs, uses curly braces and colons | { name: 'Paul', age: 40} |


# Numeric Operators
| Operation	| Code | Math |
| --------- | ---- | ---- |
| Addition	| 5 + 2	| 5 + 2 = 7 |
| Subtraction	| 5 - 2	| 5 - 2 = 3 |
| Multiplication	| 5 * 2	| 5 x 2 = 10 |
| Division	| 5 / 2	| 5 / 2 = 1.5 |
| Floor Division	| 5 // 2	| ⌊5/2⌋ = 1 |
| Modulus Division	| 5 % 2	| 5 mod 2 = 1 |
| Negation	| -2	| -2 |
| Exponent	| 5 ** 2	| 52 = 25 |
| Absolute Value |abs(-2)	| \|-2\| = 2 |
| Square Root*	| Math.sqrt(2)	| √2 |

\* requires that the Math module is already imported


# Boolean Expressions
All expressions can be interpreted as a Boolean value.  The following all evaluate to False:

    - None
    - False  (which is already a Boolean value)
    - 0  (whatever type from integer, float to complex)
    - Empty collections:   "", (), [], {}
    - Objects with the special method __nonzero__
    - Objects that implement __len__ to return False or zero

All other expressions evaluate to True.

| Expression	| Description |
| ---- | ---- |
| a == b	| True if a and b are equal to each other |
| a != b	| True if a and b are *not* equal |
| a is b	| True if a and b are identical |
| a is not b |	True if a and b are *not* identical |
| a > b |	True if a is greater than b |
| a >= b	| True if a is greater than or equal to b |
| a < b	| True if a is less than b |
| a <= b |	True if a is less than or equal to b |
| a in x	| True if x is a collection that contains a |
| a not in x	| True if x is acollection that does *not* contain b |
| not a	| True if a is False |

Boolean expressions can be combined with and/or:

| Expression	| Description |
| ---- | ---- |
| a and b	| True if a and b are both True |
| a or b	| True if either a or b or both are True |


# Variables and Types
All variables have a type at any given time, although that type can change during the execution of the program.

```python
x = 1       # x is an integer object (1)
y = 2       # y is also an integer object (2)
z = x + y   # z is an integer (3)
a = y       # a is an integer equal to y (3)
y = "2"     # y is now changed to a string ('2')
z = x + a   # z is still an integer (4)
z = x + y   # throws a type mismatch (TypeError)
```


# Indexes and Slices
| Expression	| Description	| Result (if x = [0,1,2,3,4]) |
| ---- | ---- | ---- |
| x[0] | First element of the sequence | 0 |
| x[1] | Second element	1 |
| x[-1] | Last element | 4 |
| x[-2] | Second to last | 3 |
| x[1:-2] | All of the elements including the second up to but not including the second to last	| [1, 2] |
| x[2:] | All of the elements from the third to the end	[2, 3, 4]
| x[:3]	| All of the elements from the beginning up to but not including the fourth	| [0, 1, 2] | 
| x[:] | All of the elements (returns a copy of x) | [0, 1, 2, 3, 4] |
| x[0:4:2] | Start at the first element, then every other one up to but not including the fifth | [0, 2] |


# Built-In Functions
A function is a small piece of code that is already implemented for you.   Python comes with a bunch of 
functions built-in.  Here are some of the most useful:

| Function Name | Description |
| ---- | ---- |
| type() | Takes an object, and tells you what kind of object it is |
| round() | Rounds a number to the nearest unit. If a second parameter is provided, rounds that many decimal places left (negative) or right (positive) of the decimal.  E.g.: ``` >>>  round(325, -2) ``` |
| str(), int(), float() | Converts an expression to the specified type: string, integer, or floating point (respectively) |
| print() | Prints a list of objects to the screen (by default) or a file (if specified). |
| input()	| Gets text from the user, if a parameter is provided, uses that value to prompt the user. |



