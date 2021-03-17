## What computer science about? 
	⁃	design algorithm
	⁃	optimize the number of operation 

## Big O
	⁃	number of operation == running time/ program / algorithm 
	⁃	keep highest depend of n, fast growing term in n, remove all constant and others 

## Searching
	⁃	searching for value(don’t know the data) —>linear search (O(n))
	1.	 x in list
	2.	list.index (x)
	⁃	searching for value(sorted data)—> binary search(O(log2n))
	⁃	begin list(b) / mid / end list(e)
	⁃	 (index b + index(e) )//2 = mid 
	⁃	if value > mid	—> index b =mid+1
	⁃	if value < mid —> index e=mid-1
## Swap
	⁃	string, int, float, tuple—> immutable 
	⁃	list, set —>mutable 
	⁃	swiping can be down create new value to contain 1 of value 
	⁃	if it is swap list, can do like: a[1]=a[0]

## Sorting  
	`1.	selection sort (n**2)`
def selection_sort(L):
   ''' sorts given list L'''
    for i in range(len(L)-1): # Find the minimum in the list[len(L)-1], the last number should be max
          index_of_min=i
          for j in range(i+1, len(L)):
              if(L[index_of_min]>L[j]):
                  index_of_min=j
          #Swap L[i] with L[index_of_min] if necessary
          # (the line of code below does basically nothing if L[i] is the minimum, i.e. if i==index_of_min)
          L[i],L[index_of_min]=L[index_of_min], L[i]
			# this also can be write as tmp=L[i] L[i]= L[index_of_min] L[index_of_min]=tmp
`2. Merge sortO(n*logn)`
recursive mergesort
```
def merge_sort(L):
    if len(L)<2:
        return L[:]
    else:
        middle =len(L)//2
        left=merge_sort(L[:middle])
        right=merge_sort(L[middle:])
        return merge(left,right)
```
```
def merge(L1, L2):
     """ (list, list) -> list
     Merge sorted lists L1 and L2 into a new list and return that new list.
     >>> merge([1, 3, 4, 6], [1, 2, 5, 7])
     [1, 1, 2, 3, 4, 5, 6, 7]
     """
     newL = []
     i1 = 0
     i2 = 0
     # For each pair of items L1[i1] and L2[i2], copy the smaller into newL.
     while i1 != len(L1) and i2 != len(L2):
          if L1[i1] <= L2[i2]:
               newL.append(L1[i1])
               i1 =i1+ 1
          else:
               newL.append(L2[i2])
               i2=i2+ 1
     # Gather any leftover items from the two sections.
     # Note that one of them will be empty because of the loop condition.
     newL.extend(L1[i1:])
     newL.extend(L2[i2:])
     return newL
```
`3. quick sort O(n**2)`
```
def qs(a):
    """Return a sorted copy of a"""
    if len(a) == 0:
        return []
    x = random.choice(a)
    lt, eq, gt=[],[],[] 
# lt = collection of number smaller then x 
# eq = collection of number equal to x 
# gt = collection of number bigger then x
    
    for item in a:
         if item < x:
             lt.append(item)
         elif item == x:
             eq.append(item)
         else:
             gt.append(item) 
    return qs(lt) + eq + qs(gt)
```
O(n*log2n)=n+(n-1)+(n-2)+(n-3)+….+1=(n+1)*n //2 

## Type of algorithm 
	1.	logarithmic O(logn) —>binary search
	2.	linear O(n)—>linear search
	3.	superlinear O(n*logn) —> heap sort, merge sort
	4.	Polynomial O(n^C) —>insertion sort/ selection sort / quick sort
	5.	Exponential O(C**n)
	6.	Factorial O(n!) 

## Recursion 
	•	max 1000 function can run at the same time 
	•	recursion depth/height in stack is 1000 
	•	recursion similar like loop, do the small part in stack 
	•	if variable does not exist in function, it goes to global variable to find
	•	‘global’ refer to global variable 
	 set within the function and before it sign to value to it
	(declare variable==global variable)



