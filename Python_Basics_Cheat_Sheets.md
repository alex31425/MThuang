
- ## Tuple


### Tuple creation :


```python
tup = 1,2,3
tup
```

    (1, 2, 3)
    


```python
tuple('ABC')
```




    ('A', 'B', 'C')



### Sequence or iterator conversion :


```python
tup = 1,2,'A',True
tup
```

    (1, 2, 'A', True)
    

### Indexing and slicong :


```python
tup[0]
```




    1




```python
tup[1:3]
```




    (2, 'A')



### Lehgth of the tuple :


```python
tup = (1,2,3,'a',True)
len(tup)
```




    5



### Unable to modify which object is stored in each slot:



```python
tup[1]=2
```


    ---------------------------------------------------------------------------

    TypeError                                 Traceback (most recent call last)

    <ipython-input-11-f2ca30833131> in <module>
    ----> 1 tup[1]=2
    

    TypeError: 'tuple' object does not support item assignment


### If the tuple contains LIST, which is mutable, the elements in the LIST can be modified:


```python
tup = (1,[1,2],3,'a',True)
tup[1][0]=3
tup 
```




    (1, [3, 2], 3, 'a', True)




```python
tup[1].append(5)
tup
```




    (1, [3, 2, 5], 3, 'a', True)



### Concatenate and Multiply a tuple :



```python
tup = (1,2,3)*2
tup
```




    (1, 2, 3, 1, 2, 3)




```python
tup = (1,2,3)
tup1 = (2,5)
tup+tup1
```




    (1, 2, 3, 2, 5)



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
## List

### In contrast with tuple, list contents can be modified in-place. A list can be created by using square brackets [ ] or using the list type function:

### Tuple creation :


```python
l = [1,2,3] 
type(l) 
```




    list



### Swutch between tuple and list:


```python
tup = ('a','b')
list(tup)
```




    ['a', 'b']



### Check if a element in a list:



```python
1 in l
```




    True



### Add, modify, and remove elements form the list



```python
l.append(7) # add element
l
```




    [1, 2, 3, 7]




```python
l[3]= 8 # modify element
l
```




    [1, 2, 3, 8]




```python
l.insert(4,10) # insert an element at a specific location in the list
l
```




    [1, 2, 3, 8, 10]




```python
l.pop(0) # removes and returns an element at a particular index
l
```




    [2, 3, 8, 10]




```python
l.remove(2) # remove elements by value
l
```




    [3, 8, 10]



### Combine & concatenate list



```python
l2 = [5,6,(8,9)]
l.extend(l2)
l
```




    [3, 8, 10, 5, 6, (8, 9)]




```python
l3 = [10,11]
l+l3

```




    [3, 8, 10, 5, 6, 10, 11]




```python
del l[5] # delete elements by their index
l
```




    [3, 8, 10, 5, 6]



### Sorting



```python
l4 = [10,9,1,5,3,2]
l4.reverse()
l4
```




    [2, 3, 5, 1, 9, 10]




```python
l4.sort()
l4
```




    [1, 2, 3, 5, 9, 10]




```python
l5 = [11,10,9,8,7,6]
print(f' New list : {sorted(l5)};\n Original list : {l5}') # returns a new sorted list
```

     New list : [6, 7, 8, 9, 10, 11];
     Original list : [11, 10, 9, 8, 7, 6]
    

### Slicing

### [Start Index:End Index] start index is included, the stop index is not included


```python
l5[1:3]
```




    [10, 9]




```python
l5[:-1]
```




    [11, 10, 9, 8, 7]




```python
l5[-3:]
```




    [8, 7, 6]
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
- https://www.w3schools.com/python/default.asp
- https://www.geeksforgeeks.org/python-programming-language/
- https://medium.com/pythonland/30-python-language-tricks-that-will-make-you-a-better-coder-f08f811a7b0f
