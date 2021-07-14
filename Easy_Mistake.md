## Traps	
	
1.	input only allow 1 argument, using plus sign (+) to concatenate to produce new string 
2.	input from user, the value returns always be string 
3.	calculator of python 
	```
	⁃	x%y —>mod return a reminder (x%y=x-(x//y)*y
	⁃	x//y —>div  return a integer 
	⁃	round(float) —> output is integer . When decimal is 0.5: if int is odd, plus 1; if int is even, no change 
	⁃	int(float) —> remove all decimal 
	⁃	math.ceil() —> up to biggest int
	⁃	math.floor()—> down to smallest int 
	⁃	math.log(x, base) 
	```
4. True and False the capital at condition 
5.  Each string all has `“ “` or ` ‘ ‘ `
6. object 
Don’t forget to write ‘self’  in each function with in the object 
	```Python
	class object_name():
		def function_name(self):
			body 
	```
Calling in object —> function_name()
7. Slicing & Range 易错点！！
如果想要count down set list/string[::-1] 
```
List/string[-2:] —> return last two items in the array 
List/string[:-2] —> return everything except last two 
List/string[::-1]—> return reverse, all items in the array 
List/string[1::-1]—> only the first two items reversed 
List/string[:-3:-1] —> the last two items, revered 
```
range(5,-1,-1)—> begin at 5, end with -1—> 5,4,3,2,1

8. List and object has aliasing 
If one got change, another one change too 

9. ``**`` is square , ``^`` isn’t 

10. List can be inside of list —> 2D list 
list[out index][inside index]

11. `is` —> compare address //  `==` compare content 

12. `List.append(x)` and `list.sort()` can’t assign to new variable 

13. Range out of index len(s) -1 

14. To solve even / odd number by increment can use plus/ minus 
Ex. i =5 # only work for odd number 
```
	while …: 
		i = i+2 # step to odd number 7,9,11…
```
15. list=[] != list=[None]
None is undetermined 
So if want set the more index in list, use None 

16. Tab character `\t` // newline character `\n`

17. Can not directly convert list<str> —> list<int>

18. After loop done, the last value will sign to I 

19. List can only concatenated with list 
list[]+list[] 

list(string) —>works for string
list(int) —>doesn’t work 

20. [1]* 10 =[1,1,1,1,1,1,1]-> without extra list 

21. 凡是在while loop 中 *2 or //2; the operation 都为 log n
ex.1 def foo1 (n): #O(logn)
```
		 x=1
		while x<n:
			x=x*2
```
ex.2 def foo2(n): #O(logn)
		```
		x=n
		while x>=1:
			x=x//2
		```
ex.3 def foo3(n): #O(n*logn)
	```
	 for x in range(n):
		j=x
		while j>=1:
			j=j//2
	```
22. How to do backwards? 
For loop : range(len(s)-1,-1,-1)
```Python
While loop: i=len(s)-1 
	while condition :
	i = i -1
```

23. If key is string, should add `“” `

24. a=[1,2,3,4,5,6,7,8,9]
a[::2] —> return a list [1,3,6,9]

25. Remember test case 0 value! Always! 
Division can’t be zero !!! X/0 doesn’t work !!!

26. Int can’t using slicing and len!!!

27. set the default to the Object init 





