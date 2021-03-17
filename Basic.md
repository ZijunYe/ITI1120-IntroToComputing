## Help() and dic()
help(function_name) —> show the usage of the function

dic(object) —> list all the function that can use with object 

## Comma(,) & Plus sign(+)

`Comma`: used to separate the value/arguments you send to function calls 
	1)	area_of_triangle(2.1,4)—>sending 2 values to function; 1 float & 1 int
	2)	print(“2*4 is”,8,”have nice day”)—>Sending 3 value to function print, 1 string,1 int, 1 string (print function default separate by space)
`Plus sign`: when applied to strings, concatenated two string to produce new string 
	⁃	ex. “2*4 is” + str(8) + “have nice day” —>  ‘2*4 is 8 have nice day’
	⁃	input () function, only allow 1 argument / parameter 

## Print & return 
	•	Print only display the output; has to have bracket “()”
	•	Return no display, but keep the value 
	•	print(“\n”) —> default setting of print 
	•	print(x, end=“”) —> print at same line

## Defining Function
def funtion_name(parameters):
	body 
	1.	def: a key word indicating a function definition 
	2.	function name: the function name 
	3.	parameters:
	⁃	the parameter(s) of the function, 0 or more and are separated by comma 
	⁃	a parameter is variable 
	4. body: 1 or more statement, often ending with a return statement

## Assignment statement 
	variable_name=expression

## Function_name(arguments/value)
Rule for executing a function call:
	1.	when call it, then function starting working 
	2.	evaluate the argument 
	3.	call the function, passing in the argument values 
Terminology 
	1.	 argument: a value given to a function
	2.	pass: to provide to a function 
	3.	call: ask python to evaluate a function
	4.	return: pass back a value 

## Using non-builtin function 
import module_name 
module_name.function_name

Modules: contains many function, but not all of them are immediately available as builtin function
Some module we usually use: 

	import math 
		- math.sqrt
	import random 
	⁃	random.shuffle(x) —> x should be has lens (such as list)
	⁃	random.randrange(stop)
	⁃	random.randrange(start,stop[,step])
	⁃	random.randint(a,b)  —> output a<= x <=b
	⁃	random.choice(x)—>random pick 1 elements from the list 
	⁃	random.sample(range(1,100),10) --> 10 is how many number to pick 
	import string  
	⁃	string.punctuation 
	⁃	x.isalpha() —> check if the words is letter 

## What is main?
	⁃	main is your program; all commands aligned with leftmost edge of your file
	⁃	function is not part of your main, only run when you call it 
	⁃	variable created in the main is global variable 

## Docstring 
	⁃	if not return any value —>None 
	⁃	if input is list: put list 
	⁃	if the function in object, ‘self’—>Object_name

## If statement
Indent is key key key!
```Python 
If condition:
	body 
elif condition:
	body
else: 
	body 
```
Rule for executing an if statement 
	1.	evaluate each expression in order from top to bottom
	2.	when one condition is true, then rest won’t work 

## Loop
`For loop `
for variable in str/numeric:
	body
`While loop `
while expression:
	statements  
	⁃	lazy evaluation —> check 1 condition matched then stop, if 1 condition is false, second operand not even evaluated 
	⁃	only stop when condition is false 
	⁃	set i outside;   incremental i at inside 
Any loop can work individually without function 

## Slicing 
- count down set list/string[::-1] 
List/string[-2:] —> return last two items in the array 
List/string[:-2] —> return everything except last two 
List/string[::-1]—> return reverse, all items in the array 
List/string[1::-1]—> only the first two items reversed 
List/string[:-3:-1] —> the last two items, revered 

## String 
	⁃	compare string base on dictionary, not length 
	⁃	it’s immutable
	⁃	 string can’t change individual letter, seem string as whole 

## list 
The collection of data(mutable) 
	⁃	len(list)
	⁃	min(list)/max(list)/sum(list)—> only inside is numerical 
	⁃	how to create list —> list_name=[]

## 2D List 
	⁃	1D list = [1,2,3,4]// 2D list=[[1,2],[3,4]]
	⁃	inside list is column, outside list is row 
	⁃	first row then column


## Tuple 
Immutable sequences: can not be modify 
(x,y )—> to create a tuple 

## Set
a collection of unordered distinct element/object
creates:  by using set()
function:
	⁃	set_name.add(element) —> can’t use append (mutable)
	⁃	set_name.remove(element)
	⁃	can’t sort by index, slicing 
	⁃	set doesn’t contain repeat value

## Dictionary 
It contains {key:value}
Key works like index; dictionary_name[key]=value 
Creates: by using {}
- how to create new key and value in dictionary 
	dictionary_name[key_name]=value 
- how to switch key and value 
	new_value=dictionary[key]
	dictionary[new_value]=key 


## Object 
class Object_name(): 
	def __init__(self, x,y):
		self.x=x
		self.y=y 
	⁃	the default of ‘x’ and ‘y’ is 0 
	⁃	first ‘self’ stored object’s address
	⁃	__init__ it calls contractor 
	⁃	Don’t forget to write ‘self’  in each function with in the object 
	⁃	class object_name():
	⁃	def function_name(self):
	⁃		body 
	⁃	Calling in object —> function_name()

## Reading File 
	⁃	open(filename) —> out put is file’s address 
	open(filename, mode) —> ‘r’ to open for read; ‘w’ to open for writing ; ‘a’ to open for appending to what is already in the file;
	⁃	flanders_file.read() —> read file as a single string 
	⁃	flanders_file.readlines()—>read and returns all lines 
	⁃	flander_file.readline()—>read and return next line of file 
	⁃	file.close()

## Computer memory 
variable=expression 
	1.	evaluate the expression. This produces a memory address
	2.	store the memory address in the variable

## Variable name — memory address — value 
	⁃	a value has a memory address
	⁃	a variable contains a memory address
	⁃	a variable refers to a value
	⁃	a variable points to a value 

## Others 
	⁃	n! —> non-negative integer/ factorial 
	⁃	n! 
	⁃	n=0  0!=1
	⁃	n>=1 n(n-1)!





