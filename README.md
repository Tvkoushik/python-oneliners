# python-oneliners
This github repo is a collection of amazing python one liners which I regularly use and feel saves a lot of time especially for complex tasks. 
Feel free to add more to the list.


# Index
* [Sort a dictionary based on multiple conditions](#Sort-a-dictionary-based-on-multiple-conditions)
* [Thousand Separator]
* [Multiply all elements of a list](#combine-two-lists-to-dictionary)
* [Flatten a List](#common-element-between-two-lists)
* [Remove duplicate elements from a list](#convert-decimal-to-binary)
* [Get quotient and remainder](#convert-decimal-to-octal)
* [Most frequent element of a List](#convert-deciaml-to-hexadecimal)
* [Convert string to upper case](#convert-deciaml-to-hexadecimal)
* [Converting string to byte](#convert-a-list-of-strings-to-integers)
* [Transpose a Matrix](#convert-key-value-pair-to-dictionary)
* [Element wise addition of 2 lists](#convert-string-to-lower-case)
* [Convert ASCII value to Character and vice versa](#convert-string-to-upper-case)
* [Print all combinations of elements in a List](#convert-string-to-bytes)
* [Input space separated integers in a list](#copy-files)
* [Nested for loops via List comprehension](#count-occurence-of-a-character-in-a-string)
* [Find All Indices of an Element in a List](#count-occurence-of-a-character-in-a-string)
* [Convert number of any base to decimal](#count-occurence-of-a-character-in-a-string)


### Sort a dictionary based on multiple conditions

```python
d={'IN':2, 'GE':2, 'AK':3, 'BEG':1}

n_l=[sorted (d.items(), key=lambda x: (x[1], len(x[0]),x[0])))

new_d={k:v for k,v in n_l} 

# new_d = {'BEG': 1, 'GE': 2, 'IN': 2, 'AK': 3}
```

### Thousand Separator
```python
n=10000000

new_number=f'{n:, }'

# new_number = 10,000,000
```
### Multiply all elements of a list
```python
from numpy_import prod from functools import reduce

1=[2,3,4,4,5,6]

v1=prod(1) # 2880 

v2=reduce((lambda x, y: x * y), 1) #2880
```

### Flatten a List
```python
1 = [[7,6], [4, 6], [8, 10]]

flattened = [i for j in 1 for i in j]

# flattened = [7, 6, 4, 6, 8, 10]
```

### Remove duplicate elements from a list
```python
1 = [4,4,5,5,6]

new_l=list(set(1))

# new_1 = [4,5,6]
```

### Get quotient and remainder
```python
quotient, remainder = divmod(10,5)

# quotient, remainder = 2,0
```

### Most frequent element of a List
```python
from collections import Counter

1 = [1,1,3,4,1,5,6,7,7,2,9]

freq_ele=Counter(1).most common()[O][O]

# freq_ele = 1
```

### Convert string to upper case
```python
"hi my name is Allwin".upper()

# 'HI MY NAME IS ALLWIN'
```

### Converting string to byte
```python
s="My name is fox and fox is an animal"

s.encode()

# b'My name is fox and fox is an animal'
```

### Transpose a Matrix
```python
martix = [[1, 2, 3], [3, 4, 6], [5, 6, 7]] 

1=list(list(x) for x in zip(*matrix))

# 1 = [[1, 3, 5], [2, 4, 6], [3, 6, 7]]
```

### Element wise addition of 2 lists
```python
first = [1,2,3,4,5]

second = [6,7,8,9,10]

final=[x + y for x, y in zip(first, second)]

# final = [7, 9, 11, 13, 15]
```

### Convert ASCII value to Character and vice versa
```
ord('a') # 97

chr(97) # a

chr(ord('a') + 3) #d
```

### Print all combinations of elements in a List
```python
from itertools import combinations, combinations_with_replacement

nums = [1,2,3,4]

list(combinations(nums, 2)) # [(1, 2), (1, 3), (1, 4), (2, 3), (2, 4), (3, 4)]

list(combinations_with_replacement(nums, 2)) # [(1, 1), (1, 2), (1, 3), (1, 4), (2, 2), (2, 3), (2, 4), (3, 3), (3, 4), (4, 4)]

list(combinations (nums, 3)) # [(1, 2, 3), (1, 2, 4), (1, 3, 4), (2, 3, 4)]
```

### Input space separated integers in a list
```python
l = list(map(int, input().split()))
```

### Read file in python and input it to a list
```python
one-liner.py
l = [line.strip() for line in open('abc.txt', 'r')]
```

### Nested for loops via List comprehension
```python
l1 = [1, 2, 3, 4]

l2 = ['a', 'b', 'c']

l = [(x, y) for x in l1 for y in l2]

# [(1, 'a'), (1, 'b'), (1, 'c'), (2, 'a'), (2, 'b'), (2, 'c'), (3, 'a'), (3, 'b'), (3, 'c'), (4, 'a'), (4, 'b'), (4, 'c')]
```

### Find All Indices of an Element in a List
```python
lst = ['a', 'v', 'a', 'c', 'z']

indices = [i for i in range(len(lst)) if lst[i]=='a']

# [0, 2]
```

### Convert number of any base to decimal
```python
int('30', 8) # 24

int('1011', 2) # 11

int('1A', 16) # 26
```
