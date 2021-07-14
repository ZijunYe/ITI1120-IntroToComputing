# Basic Operation 

## 0 Variable Type 
int()
str()
float()
set()
list()

## 1 Algebraic Operator
```
+,-,*,**,/,//,%
math.ceil--->up biggest int
math.floor--->down smallest int
math.log(x,base)
round()--->depends decimal (when decimal = 0.5, odd int go up by 1, even int nonchange)
int()--->no decimal
```
## 2 Comparison Operator
```
<,>,==,<=,>=,!=
```

## 3 Boolean operators

    True,False,None

    and, or, not

## 4 indexing and slicing
### index:
    
    (0)---->(len(s)-1)

    -len(s)--->(-1)

### slicing:
    s[x:y:z]

    x-begin y-end z-skip

## 5 range
    for i in range(start,stop,skip)

## 6 list method
```
list.append(object)
list.extend([list])
list.pop(index)--->remove last,return the value of the index
list.remove(object)--->remove first appearance of object, if does exist:crash
list.reverse()
list.sort()--> return none, orginal list got changed
sorted(list)-->return a new list that could send to new variable
list.insert(int,object)
list.count(object)
list.index(object)--->crash if it does not exist
list1.extend(list1 or other list)--> repeat or add new elements into list1
```
## 7 string operator
    str1 +str2  --> making a new words

    str1 * int1 --> make a copies of the words

    int1 * str1-->concatenate copies

## 8 string method
```
s.capitalize()-->1st character capitalized
s.count(target)
s.find(target)
s.lower() / s.upper()
s.replace(old,new)
s.split('')--->split default is white space
s.splitlines() --> split at \n
s.strip()--->remove trailing white space
```
```
imort string
string.isalpha() --> check if the string only contain alphabet letter
string.isdigit()-->check if the string is digit 
```
both list and str
```
range(x,y,z) --> begin, end,step
slicing[x:y:z] --> return a list
indexing[i]
len(s)
x in s
x not in s
lst1 +lst2 / str1 + str2
lst * int ---> return copy of lst without extra list[]
str * int ---> return copy of string

```
## 9 escape character

    \n ->newline

    \t ->tab

    \\ ->backslash

    \''-> quote

## 10 dictionary operator

    d.items() view of (key,value) in d as tuple

    d.get(k) == d[k] return value

    d.keys() -returns all keys of d

    d.pop(k) removes the (key,value) with key from d, returns it value

    d.update(d2) add (key,value) pairs of d2 to d

    d.values() -return all value of d

## 11 set operator

    set1.union(set2)--> return a set that has set1 and set2 combination

    set1.intersection(set2) --> return a set that common in set1 and set2

    set_name.remove(element)

    set_name.add(elemnt)

## 12object method
```
__init__(self)--> initialize the object
__repr__(self)-->print exactly same of statement
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
<type>.__init__(x)--><type>(x)
```

## 13. Reading Files
```
open(filename)
file.readline()--> only 1 lines
file.readlines()--> return list of lines
```

## 14. avoiding error
```
try:
    body
except[could add what type of error]:
    body
```
## 15. random

    import random

    random.shuffle(x) —> x should be has lens (such as list)

    random.randrange(stop)

    random.randrange(start,stop[,step])

    random.randint(a,b)  —> output a<= x <=b

    random.choice(x)—>random pick 1 elements from the list

    random.sample(range(1,100),10) --> 10 is how many number to pick












