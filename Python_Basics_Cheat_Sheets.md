
- Tuple
<br> 
A tuple is a sequence and the elements in tuple are ordered and immutable. 
1. Tuple creation : 
<br>
`tup = 1,2,3`
<br>
`tup = 1,2,'A',True` # contain different types of element
<br>
2. Sequence or iterator conversion :
<br>
`tuple('ABC') = ('A', 'B', 'C')`
<br>
3. Indexing and slicong : 
<br>
`tup[0] = 1` ; `tup[1:2] = (2,3)`
<br>
4. Lehgth of the tuple : 
<br>
`tup = (1,2,3,'a',True) ; len(tup) = 5`
<br>
5. Unable to modify which object is stored in each slot: 
<br>
`tup[1]=2 , TypeError: 'tuple' object does not support item assignment `
<br>
6. If the tuple contains LIST, which is mutable, the elements in the LIST can be modified: 
<br>
`tup = (1,[1,2],3,'a',True) ; tup[1][0]=3` ; 
<br>
`tup = (1, [3, 2], 3, 'a', True)`
<br>
`tup[1].append(5)=>tup = (1, [3, 2, 5], 3, 'a', True)`
<br>
7. Concatenate and Multiply a tuple : 
<br>
`tup = (1,2,3)*2 = (1, 2, 3, 1, 2, 3) ; tup = (1,2,3), tup1 = (2,5), tup+tup1 = (1, 2, 3, 2, 5)`
<br>

---

- List
<br>
In contrast with tuple, list contents can be modified in-place. A list can be created by using square brackets [] or using the list type function:
1. Tuple creation : 
<br>
`l = [1,2,3] ; type(l) = list ;`
2. Swutch between tuple and list:
<br>
`tup = ('a','b'), list(tup)=['a', 'b']` 
<br>
3. Check if a element in a list:
<br>
`1 in l => True`
<br>
4. Add, modify, and remove elements form the list
<br>
`l.append(7)=>[1, 2, 3, 7]` # add element
<br>
`l[3]= 8=>[1, 2, 3, 8]` # modify element
<br>
`l.insert(4,10)=>[1, 2, 3, 8, 10]` # insert an element at a specific location in the list
<br>
`l.pop(0)=>[2, 3, 8, 10]`   # removes and returns an element at a particular index
<br>
`l.remove(2)=>[3, 8, 10]` # remove elements by value
<br>
5. Combine & concatenate list
<br>
`l2 = [5,6,(8,9)] ; l.extend(l2) ; l=>[2, 3, 10, 5, 6, (8, 9)]` 
<br>
`l3 = [10,11] ; l+l3=>[2, 3, 10, 5, 6, (8, 9), 10, 11]`
<br>
`del l[5]=>[2, 3, 5, 6, 10]` # delete elements by their index
<br>
6. Sorting 
<br>
`l.reverse()=>[10, 6, 5, 3, 2]`
<br>
`l.sort()=>[2, 3, 5, 6, 10]`
<br>
`sorted(l)` # returns a new sorted list
7. Slicing
<br>
[Start Index:End Index] start index is included, the stop index is not included
<br>
`l[1:3]=>[3, 5] ; l[:-1]=>[2, 3, 5, 6] ; l[-3:]=>[5, 6, 10]`
<br>
<figure>
    <img src="images/Slicing.jpg?raw=true"/>
    <figcaption><a href="https://www.geeksforgeeks.org/python-list/">Image source</a></figcaption>
</figure>
<br>

---
- Dictionary
1. create a dictionary
<br>
`d = {'a':1,'b':2}=>{'a': 1, 'b': 2}` or 
<br>
`d1 = dict(a=1,b=2)=>{'a': 1, 'b': 2}`
<br>
2. access and insert elements
<br>
`d['a']=>1` ; 
<br>
`d['c']=3 , d= {'a': 1, 'b': 2, 'c': 3}`
<br>
`d.get('c')=>3`
<br>
3. delete values
<br>
`del d['a']=>{'b': 2, 'c': 3}`
<br>
`d.pop('b')=>2` # return the deleted value
<br>
4. items(), keys(), values() methods
<br>
`d1.values()=>dict_values([1, 2])`
`d1.keys()=>dict_keys(['a', 'b'])`
`d1.items()=>dict_items([('a', 1), ('b', 2)])`

---
- Set
<br>
A set is an unordered collection of unique elements.
<br>
1. create a set
<br>
`s = {1,1,2,3,3,4,5}=>{1, 2, 3, 4, 5}` or
`s1 = set([1,1,2,3,3,4,5])=>{1, 2, 3, 4, 5}`
<br>
2. set operations
<br>
`s.union(b`) or `s | s1`
<br>
`s.remove(x)`
<br>
`s.pop()`
<br>
`s.intersection(s1)` or `s & s1`
<br>
`s.difference(s1)` or `s - s1`
<br>
`s.symmetric_difference(s1)` or `s ^ s1`
<br>


---

Reference :
- https://towardsdatascience.com/essential-python-every-data-scientist-should-know-in-2021-65e571c20d19
- https://realpython.com/tutorials/basics/
- https://blog.finxter.com/collection-5-cheat-sheets-every-python-coder-must-own/
