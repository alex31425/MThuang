
- Tuple
<br> 
A tuple is a sequence and the elements in tuple are ordered and immutable. 
1. Tuple creation : 
`tup = 1,2,3`
<br>
`tup = 1,2,'A',True` # contain different types of element
<br>
2. Sequence or iterator conversion : 
`tuple('ABC') = ('A', 'B', 'C')`
<br>
3. Indexing and slicong : 
`tup[0] = 1` ; `tup[1:2] = (2,3)`
<br>
4. Lehgth of the tuple : 
`tup = (1,2,3,'a',True) ; len(tup) = 5`
<br>
5. Unable to modify which object is stored in each slot: 
`tup[1]=2 , TypeError: 'tuple' object does not support item assignment `
<br>
6. If the tuple contains LIST, which is mutable, the elements in the LIST can be modified: 
`tup = (1,[1,2],3,'a',True) ; tup[1][0]=3 ; tup = (1, [3, 2], 3, 'a', True)`
<br>
`tup[1].append(5) ; tup = (1, [3, 2, 5], 3, 'a', True)`
<br>
7. Concatenate and Multiply a tuple : 
`tup = (1,2,3)*2 = (1, 2, 3, 1, 2, 3) ; tup = (1,2,3), tup1 = (2,5), tup+tup1 = (1, 2, 3, 2, 5)`

<br>
---
- List
<br>
In contrast with tuples, lists are variable-length and their contents can be modified in-place. You can define them using square brackets [] or using the list type function:
---
- Dict
---
- Set
---
- List, Set, and Dict Comprehensions

Reference :
- https://towardsdatascience.com/essential-python-every-data-scientist-should-know-in-2021-65e571c20d19
- https://realpython.com/tutorials/basics/
- https://blog.finxter.com/collection-5-cheat-sheets-every-python-coder-must-own/
