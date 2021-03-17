# Object (L18,19,20)
## Base
	1.	class Name: —> the way to create the object // Capital of first letter // mutable 
	2.	type contract of self (address of object) is object’s name 
	3.	call function that in the object either Class_name.method(self, v1,v2) // instance.method(v1,v2) 

## The steps of class
	1.	creates an object of type point 
	2.	calls an object __init__ method (initial object)
	3.	produces an object’s memory address 
	4.	variable inside of object are called instance variable


## Characteristics of Object
`1 Reference`
Class has aliasing, it could refer to the same class 
Ex. 
```Python
Class Point:
	def __init__(self, x,y):
		self.x=x
		self.y=y
a=Point(-1,1)
b=Point(3,3)
a=b
a.x=1
print(a.x, a.y, b.x, b.y)
```
Output: 1,3,1,3

`2Method `

Asigning to new variable using dot operator self.variable_name=value
```
__init__(self)--> initialize the object
repp(self)-->print exactly same of statement
__str__(self)--> when call 'print()' function shows human readable
__len__(self)-->len(s) call it classical way
__add__(self)--> x+y
__sub__(self)-->x-y
__mul__(self)-->x*y
__truediv__-->x/y
__floordiv__-->x//y
__mod__-->x%y
__eq__-->x==y
__ne__-->x!=y
__gt__-->x>y
__ge__-->x>=y
__lt__-->x<y
__le__-->x<=y
```
` 3 Inheritance`
1. class Object_name( other object name): —> it can be inheritance by other, it can put multiple object
2. Object has generic inheritance 
3. inheritance one particular function that come from other object
	> using two ways (extending)
	
	> super().other_object_function_name(x,y)
	
	> other_object _name.function(self, x,y)


