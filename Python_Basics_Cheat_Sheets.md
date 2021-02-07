- ## [Tuple](#tuple) <a id='Tuple'></a> 
- ## [List](#list) <a id='List'></a>
- ## [Dictionary](#dictionary) <a id='Dictionary'></a>
- ## [Set](#set) <a id='Set'></a>

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

- ## List


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
- ## Dictionary


### create a dictionary



```python
d= {'a': 1, 'b': 2, 'c': 3} # first method
d1 = dict(a=1,b=2) # second method
d,d1
```




    ({'a': 1, 'b': 2, 'c': 3}, {'a': 1, 'b': 2})



### access and insert elements



```python
d['a']
```




    1




```python
d['c']
```




    3




```python
d.get('c')
```




    3



### delete values



```python
del d['a']
d
```




    {'b': 2, 'c': 3}




```python
d.pop('b')  # return the deleted value
```




    2



### items(), keys(), values() methods


```python
d1.values()
```




    dict_values([1, 2])




```python
d1.keys()
```




    dict_keys(['a', 'b'])




```python
d1.items()
```




    dict_items([('a', 1), ('b', 2)])

---
- ## Set


### A set is an unordered collection of unique elements.


### create a set



```python
s = {1,1,2,3,3,4,5} # first method
s1 = set([1,2,3,4,5,6,7]) # second method
s,s1
```




    ({1, 2, 3, 4, 5}, {1, 2, 3, 4, 5, 6, 7})



### set operations


```python
s.union(s1) # first method
s | s1 # second method
print(f' first method : {s.union(s1) },\n second method : {s | s1}')
```

     first method : {1, 2, 3, 4, 5, 6, 7},
     second method : {1, 2, 3, 4, 5, 6, 7}
    


```python
s.remove(5)
s
```




    {1, 2, 3, 4}




```python
s.pop() # return the deleted value

```




    1




```python
s.intersection(s1) # first method
s & s1 # second method 
print(f' first method : {s.intersection(s1)},\n second method : {s & s1}')
```

     first method : {2, 3, 4},
     second method : {2, 3, 4}
    


```python
s1.difference(s) # first method
s1 - s  # second method 
print(f' first method : {s.difference(s1)},\n second method : {s - s1}')
```

     first method : set(),
     second method : set()
    


```python
s.symmetric_difference(s1) # first method
s ^ s1 # second method 
print(f' first method : {s.symmetric_difference(s1)},\n second method : {s ^ s1 }')
```

     first method : {1, 5, 6, 7},
     second method : {1, 5, 6, 7}


---

Reference :
- https://towardsdatascience.com/essential-python-every-data-scientist-should-know-in-2021-65e571c20d19
- https://realpython.com/tutorials/basics/
- https://blog.finxter.com/collection-5-cheat-sheets-every-python-coder-must-own/
- https://www.w3schools.com/python/default.asp
- https://www.geeksforgeeks.org/python-programming-language/
- https://medium.com/pythonland/30-python-language-tricks-that-will-make-you-a-better-coder-f08f811a7b0f
