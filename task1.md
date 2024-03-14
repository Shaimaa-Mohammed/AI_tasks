```python
#1-Write a Python program to calculate the length of a string using 2 ways
```


```python
x=input()
print(len(x))
```

    wertyuil;
    9
    


```python
y=input()
sum=0
for i in y:
    sum+=1
print(sum)
    
```

    3167egdd
    8
    


```python
#2-Write a Python program to get a string made of the first 2 and last 2 characters of a given string. If the string 
```


```python
f=input()
if len(f)< 2:
    print(" ")
else:
    print(f[0:2] + f[-2:]) 
```

    er
    erer
    


```python
#3-Write a Python program to add 'ing' at the end of a given string (length should be at least 3). If the given string already ends with 'ing', add 'ly' instead. If the string length of the given string is less than 3, leave it unchanged.
```


```python
a=input()
b=len(a)
if b > 2:
    if a[-3:] == 'ing':
        a += 'ly'
    else:
        a += 'ing'
print(a) 
```

    sdfgh
    sdfghing
    


```python
#4-Write a Python function that takes a list of words and return the longest word and the length of the longest one
```


```python
l=input()
li=l.split()
lis=[str(word) for word in li] 
x=-1
for word in lis:
    if len(word) > x:
        x=len(word)
        res=word
print("Longest word: ",res,"\n","Length of the longest word: ",x)
        
```

    errt gf ygfaa hufdsaz uyt
    Longest word:  hufdsaz 
     Length of the longest word:  7
    


```python
#**5-Write a Python program to change a given string to a newly string where the first and last chars have been 
```


```python
s=input()
r=s[-1]+s[1:-1]+s[0]
print(r)
```

    ABCD
    DBCA
    


```python
#**6-Write a Python program to remove characters that have odd index values in a given string (Sample String:abca Expected Result:ac)
```


```python
p=input()
s=""
for i in range(len(p)):
    if i % 2 == 0:#remov characters that have odd index values in a given string
        s=s+p[i] 
        
print(s) 
        
        
```

    sdfgh
    sfh
    


```python
#-7Write a Python program to count the occurrences of each word in a given sentence
(Sample String:amr and ahmed are frindes but amr is the tallest 
```


```python
def counte_occurrences_of_each_word(sentence):
        count=dict()
        word=sentence.split()
        for c in word:
            if c in count:
                count[c] += 1
            else:
                count[c] = 1 
        return count

x=counte_occurrences_of_each_word("no risk no fun")
                
x              
                
            
            
 
 
```




    {'no': 2, 'risk': 1, 'fun': 1}




```python
#**8-Write a Python script that takes input from the user and displays that input back in upper and lower cases
```


```python
script=input()
print(script.lower(),script.upper()) 
```

    dfgh
    dfgh DFGH
    


```python
#**9-Write a Python function to reverse a string if its length is a multiple of 4
```


```python
string=input()
if len(string) % 4 == 0:
    print(''.join(reversed(string)))    
```

    rtyu
    uytr
    


```python
#**10- Write a Python program to remove a newline in Python
```


```python
g="shaimaa\n"
#print(g)
print(g.rstrip())
```

    shaimaa
    


```python
#*11-Write a Python program to check whether a string starts with specified characters
```


```python
y=input()
if y[0:2] == "sh":
    print(True)
else:
        print(False)
```

    sh
    True
    


```python
#**12- Write a Python program to add prefix text to all of the lines in a string
```


```python
from functools import reduce
s = ['ANA']
pre = 'ANA_MSH_'
res = reduce(lambda res, item: res + [pre + item], s, [])
res
```




    ['ANA_MSH_ANA']




```python
#**13-Write a Python program to print the following numbers up to 2 decimal places
```


```python
i=434324.343434221214
print("{:.2f}".format(i))

```

    434324.34
    


```python
#**14-Write a Python program to print the following numbers up to 2 decimal places with a sign
```


```python
i=434324.343434221214
print("{:+.2f}".format(i))
```

    +434324.34
    


```python
#*15-Write a Python program to display a number with a comma separator
```


```python
q=20000000
print("{:,}".format(q))
```

    20,000,000
    


```python
#**16-Write a Python program to reverse a string using 2 ways
```


```python
rt="shaimaa."
print(''.join(reversed(rt))) 
print(rt[::-1])
```

    .aamiahs
    .aamiahs
    


```python
#**17-Write a Python program to count repeated characters in a string (hint:use dictionary)
```


```python
def re(s):
    x = {}
    for i in input:
        x[i] = x.get(i,0)+ 1
    return x
print(count('shaimaaa')) 
#نعد كله ميضرش
```

    {'s': 1, 'h': 1, 'a': 4, 'i': 1, 'm': 1}
    


```python
#**18-Write a Python program to find the first non-repeating character in a given string
```


```python
s="shaimaa"
for c in s:
    if(s.find(c,(s.find(c)+1)))==-1:
        print(c)
        break
```

    s
    


```python
#**19-Write a Python program to remove spaces from a given string
```


```python
i=input()
i=i.replace(" ","")
print(i)

```

    sdf tyu uuyg
    sdftyuuuyg
    


```python
#*20-Write a Python program to count the number of non-empty substrings of a given string
```


```python
l=input()
print(int(len(l)*(len(l)+1)/2))
```

    abcd
    10
    


```python
#**21-write a Python program to swap first and last element of any list.

```


```python

def swapList(blabla):
     
    f = blabla.pop(0)   
    l = blabla.pop(-1)
     
    blabla.insert(0, l)  
    blabla.append(f)   
     
    return blabla
nt = [6,2,3,5,2,1,4]
 
print(swapList(nt))
```

    [4, 2, 3, 5, 2, 1, 6]
    


```python
#**22-Given a list in Python and provided the positions of the elements, write a program to swap the two elements in the list. (Input : List = [23, 65, 19, 90], pos1 = 1, pos2 = 3
Output : [19, 65, 23, 90])
```


```python
def swapList(blabla):
     
    f = blabla.pop(0)   
    l = blabla.pop(-2)
     
    blabla.insert(0, l)  
    blabla.append(f)   
     
    return blabla
nt = [23, 65, 19, 90]
 
print(swapList(nt))
```

    [19, 65, 90, 23]
    


```python
#**23- search for the all ways to know the length of the list
```


```python
o=[2,3,4,5,13,3] 
print(len(o))
sum=0
for i in o:
    sum+=1
print(sum)
#لو علي الطرق فهيا كتيره بس الدنيا صعبه
```

    6
    6
    


```python
#**24-write a Python code to find "the Maximum number of list of numbers"
```


```python
list_of_numbers=[2,3,1,77,3]
list_of_numbers.sort()
print("the Maximum number of list of numbers is",(list_of_numbers[-1])) 

```

    the Maximum number of list of numbers is 77
    


```python
#**25-write a Python code to find the Minimum number of list of numbers.
```


```python
list_of_numbers=[2,3,1,77,3]
list_of_numbers.sort()
print("the Minimum  number of list of numbers is",(list_of_numbers[0])) 

```

    the Minimum  number of list of numbers is 1
    


```python
#*26-search for if an elem is existing in list
```


```python
l=[3,2,1,4,5,63,2]
x=0
if x in l:
    print("exit")
else:
    print("not exist") 
```

    3
    not exist
    


```python
#**27- clear python list using different ways
```


```python
p=[1,63,32,234]
p.clear()
print(p)
#مفيش احسن من كلير
```

    []
    


```python
#*28-remove duplicated elements from a list
```


```python
o=[24,1,4,21,4,1] 
d=set(o)
print(list(d))
```

    [24, 1, 4, 21]
    


```python
#**29-Given list values and keys list, convert these values to key value pairs in form of list of dictionaries.



 test_list = ['Gfg', 3, 'is', 8], key_list = ['name', 'id']
Output : [{‘name’: ‘Gfg’, ‘id’: 3}, {‘name’: ‘is’, ‘id’: 8}])
```


```python
test_list = ['Gfg', 3, 'is', 8]
key_list = ['name', 'id']
res = [{key_list[i]: val for i, val in enumerate(pair)} for pair in zip(test_list[::2], test_list[1::2])]
print(str(res))

```

    [{'name': 'Gfg', 'id': 3}, {'name': 'is', 'id': 8}]
    


```python
#**30-write a python program to count unique values inside a list using different ways
```


```python
l = [7,4,7,2,3,4,3,7]
s = set(l)
len(s)
#نعمه وفضل لو الطريقه الوحيده صح
```




    4




```python
#**31-write a python program Extract all elements with Frequency
greater than K (Input : test_list = [4, 6, 4, 3, 3, 4, 3, 4, 3, 8], K = 3 
Output : [4, 3] )
```


```python
from collections import Counter
 
test_list = [4, 6, 4, 3, 3, 4, 3, 7, 8, 8]
K = 2
f = Counter(test_list)
res = list(filter(lambda i: f[i] > K, f))
str(res)
```




    '[4, 3]'




```python
#**32-write a python program to find the Strongest Neighbour
(Input: 1 2 2 3 4 5
Output: 2 2 3 4 5)
```


```python
l1=[1,2,2,3,4,5] 
l2=[]

for i in range(1,len(l1)):
    m=max(l1[i],l1[i-1])
    l2.append(m)
for i in l2:
    print(i)
    
```

    2
    2
    3
    4
    5
    


```python
#**33-write a Python Program to print all Possible Combinations from the three Digits 
```


```python
'''l=input()
li=l.split()
lis=[int(num) for num in li] 
if len(lis)==3 :
    
    for x in range(len(lis)): 
        for y in range(len(lis)): 
            for z in range(len(lis)):
                if x!=y & y!= z & z!=x :
                    print(lis[x],lis[y],lis[z])
else:
        print("the length of list must equal tree") '''
my_list=[1,2,3]
A=[
            [my_list[0],my_list[2],my_list[1]],
            [my_list[1],my_list[0],my_list[2]],
            [my_list[2],my_list[1],my_list[0]]
        ]

for rows in A:
    print(rows)
for col in range(len(A[0])):
    column=[A[row][col] for row in range(len(A))]
    print(column)
    
```

    [1, 3, 2]
    [2, 1, 3]
    [3, 2, 1]
    [1, 2, 3]
    [3, 1, 2]
    [2, 3, 1]
    


```python
#**34-write a Python program to find all the Combinations in the list with the given condition (Input: test_list = [1,2,3] 
Output: 
 [1], [1, 2], [1, 2, 3], [1, 3]
 [2], [2, 3], [3])
```


```python
my_list=[1,2,3]
A=[
            [my_list[0],my_list[1],my_list[2]],
            [my_list[2],my_list[1],my_list[1]],
            [my_list[0],my_list[2],my_list[0]]
        ]
s1=[]
s2=[]
s3=[]
s1.append(my_list[0])
s2.append(my_list[1])
s3.append(my_list[2])
print(A[0])
print(A[0][1::])
print(A[0][0:2])
print(A[2][0:2])
print(s1)
print(s2)
print(s3)
```

    [1, 2, 3]
    [2, 3]
    [1, 2]
    [1, 3]
    [1]
    [2]
    [3]
    


```python
#*35-write a Python program to get all unique combinations of two Lists (List_1 = ["a","b"]
List_2 = [1,2]
Unique_combination = [[('a',1),('b',2)],[('a',2),('b',1)]] )
```


```python
l1 = ["a","b"]
l2 = [1,2]
 
uc=[]
 
for x in range(len(l1)):
    for y in range(len(l2)):
        uc.append((l1[x], l2[y]))
uc
```




    [('a', 1), ('a', 2), ('b', 1), ('b', 2)]




```python
#**36-Remove all the occurrences of an element from a list in Python (Input : 1 1 2 3 4 5 1 2 1 

**Output : 2 3 4 5 2)
```


```python
l = [1,1,2,3,4,5,1,2,1]  
r=1
o=[y for x,y in enumerate(l) if y!=r]  
print(o)
```

    [2, 3, 4, 5, 2]
    


```python
#**37-write a python program to Replace index elements with elements in Other List
(The original list 1 is : [‘Gfg’, ‘is’, ‘best’] The original list 2 is : [0, 1, 2, 1, 0, 0, 0, 2, 1, 1, 2, 0] The lists after index elements replacements is :
[‘Gfg’, ‘is’, ‘best’, ‘is’, ‘Gfg’, ‘Gfg’, ‘Gfg’, ‘best’, ‘is’, ‘is’, ‘best’, ‘Gfg’])
```


```python
import numpy as np
test_list1 = ['Gfg', 'is', 'best']
test_list2 = [0, 1, 2, 1, 0, 0, 0, 2, 1, 1, 2, 0]
res = np.take(test_list1, test_list2)
str(res)
```




    "['Gfg' 'is' 'best' 'is' 'Gfg' 'Gfg' 'Gfg' 'best' 'is' 'is' 'best' 'Gfg']"




```python
#ما اناا كان لازم احول بردو
```


```python
#*38- write python program to Retain records with N occurrences of K(Input : test_list = [(4, 5, 5, 4), (5, 4, 3)], K = 5, N = 2 
Output : [(4, 5, 5, 4)]
Input : test_list = [(4, 5, 5, 4), (5, 4, 3)], K = 5, N = 3 
Output : [] )
```


```python
#39-write a Python Program to Sort the list according to the column using lambda

```


```python
def sort_according_column(array):
        for i in range(len(array)):
            res=sorted(array,key=lambda A:A[i])
            print("Sorted array specific to column",i,res)
sort_according_column([[1, 3, 3], [2, 1, 2], [3, 2, 1]])

```

    Sorted array specific to column 0 [[1, 3, 3], [2, 1, 2], [3, 2, 1]]
    Sorted array specific to column 1 [[2, 1, 2], [3, 2, 1], [1, 3, 3]]
    Sorted array specific to column 2 [[3, 2, 1], [2, 1, 2], [1, 3, 3]]
    


```python
#*40- write a program to Sort Python Dictionaries by Key or Value
```


```python
di={'ravi': 10, 'rajnish': 9, 'sanjeev': 15, 'yash': 2, 'suraj': 32}
k=list(di.keys())
k1=k.sort()
s={x: di[x] for x in k}
print(s)
```

    {'rajnish': 9, 'ravi': 10, 'sanjeev': 15, 'suraj': 32, 'yash': 2}
    


```python
#**41-write python program to Remove keys with Values Greater than K ( Including mixed values )
```


```python
tes = {'Gfg' : 3, 'is' : 7, 'best' : 10, 'for' : 6, 'geeks' : 'CS'}
kt=list(tes.values())
K=7
res = {k : v for k, v in tes.items() if not (isinstance(v, int) and (v >= K))}
str(res)
            
```




    "{'Gfg': 3, 'for': 6, 'geeks': 'CS'}"




```python
#42-Write a Python program to concatenate the following dictionaries to create a new one
```


```python
dic1={1:10, 2:20}
dic2={3:30, 4:40}
dic3={5:50,6:60}
dic=dic1|dic2|dic3
print(dic)
```

    {1: 10, 2: 20, 3: 30, 4: 40, 5: 50, 6: 60}
    


```python
#**43-Write a Python program to iterate over dictionaries using for loops
```


```python
dit={"age":11,"a":4,"ag":44}
for k,v in dit.items():
        print(k,"  ",dit[k])
```

    age    11
    a    4
    ag    44
    


```python
#**44- Write a Python script to merge two Python dictionaries
```


```python
d1={"age":11,"ablaaa":4,"ag":44}
d2={"treretre":11,"nenene":4,"blabla":44}
d3=d2.copy()
d3.update(d1)
print(d3)
```

    {'treretre': 11, 'nenene': 4, 'blabla': 44, 'age': 11, 'ablaaa': 4, 'ag': 44}
    


```python
#**45-Write a Python program to get the maximum and minimum values of a dictionary values
```


```python
d2={"treretre":11,"nenene":4,"blabla":44}
dede=list(d2.values())
x=-1
vb=10000.44
for trere in dede:
    if trere > x:
        x=trere
        ma=trere
    elif trere < vb:
        vb=trere
        mi=trere
        
print(ma,"\n",mi)
    
```

    44 
     4
    


```python
**46- Write a Python program to drop empty items from a given dictionary.
Original Dictionary:
{'c1': 'Red', 'c2': 'Green', 'c3': None}
New Dictionary after dropping empty items:
{'c1': 'Red', 'c2': 'Green'}
```


```python
O={'c1': 'Red', 'c2': 'Green', 'c3': None}
O={k:v for (k,v) in O.items() if v is not None}
print(O)
        
```

    {'c1': 'Red', 'c2': 'Green'}
    


```python
#*47-Write a Python program to create a tuple of numbers and print one ite
```


```python
t=(1,3,2)
print(t[0])
```

    1
    


```python
#**48-Write a Python program to unpack a tuple into several variables
```


```python

```


```python
#**49-Write a Python program to add an item to a tuple
```


```python
t=(3,4,12,2) 
l=list(t)
l.append(543)
t=tuple(l)
print(t)
```

    (3, 4, 12, 2, 543)
    


```python
#**50-Write a Python program to convert a tuple to a string
```


```python
tpl=(2,3,4,1,2)
tpl=str(tpl)
print(type(tpl),tpl)  
```

    <class 'str'> (2, 3, 4, 1, 2)
    


```python
#**51-Write a Python program to convert a list to a tuple
```


```python
lst=[2,3,4,5,2,1,2]
type(lst)
lst=tuple(lst)
print(type(lst),lst) 
```

    <class 'tuple'> (2, 3, 4, 5, 2, 1, 2)
    


```python
#**52-Write a Python program to reverse a tuple
```


```python
tup=(1,2,4,73,45,7,6)
tup=list(tup)
tup.reverse()  
tup
```




    [6, 7, 45, 73, 4, 2, 1]




```python
#**53-Write a Python program to replace the last value of tuples in a list.
Sample list: [(10, 20, 40), (40, 50, 60), (70, 80, 90)]
Expected Output: [(10, 20, 100), (40, 50, 100), (70, 80, 100)]
```


```python
lis=[(10, 20, 40), (40, 50, 60), (70, 80, 90)]
s1=list(lis[0])
s1[-1]=100
s1=(s1)
s2=list(lis[1])
s2[-1]=100
s2=tuple(s2)
s3=list(lis[2])
s3[-1]=100
s3=tuple(s3)
lis.clear()
lis.append(s1)
lis.append(s2)
lis.append(s3)
lis

```




    [[10, 20, 100], (40, 50, 100), (70, 80, 100)]




```python
#*54-Write a Python program to convert a given string list to a tuple
Original string: python 3.0
<class 'str'>
Convert the said string to a tuple:
('p', 'y', 't', 'h', 'o', 'n', '3', '.', '0')
```


```python
s="python 3.0"
t=tuple(i for i in s if not i.isspace())
print(t)

```

    ('p', 'y', 't', 'h', 'o', 'n', '3', '.', '0')
    


```python
#**55-Write a Python program to calculate the average value of the numbers in a given tuple of tuples
```


```python
t=(1,2,3) 
s=list(t) 
sum=0
for i in range(len(t)):
    if i < len(t):
        sum+=t[i]
    else:
        break
print((sum)/(len(t)))
```

    2.0
    


```python
#56-Write a Python program to add member(s) to a set.
```


```python
se={[1,2,3,3]} 
se.add(33)
se 
#حاسه قصده مش كده بس بيس
```




    {1, 2, 3, 33}




```python
#**57-Write a Python program to remove an item from a set if it is present in the set.
```


```python
s={2,3,42,3,2}
s.clear()
s
```




    set()




```python
#**58-Write a Python program to create an intersection,union,difference and symmetric difference of sets

```


```python
a={2,4,6,2,57,6,4}
b={3,5,2,7,2,1,0,55,3}
print("intersection = ", a&b)
print("union = ", a|b)
print("difference = " , a-b)
print("symmetric difference = ", a^b) 
```

    intersection =  {2}
    union =  {0, 1, 2, 3, 4, 5, 6, 7, 55, 57}
    difference =  {57, 4, 6}
    symmetric difference =  {0, 1, 3, 4, 5, 6, 7, 55, 57}
    


```python
#*59-Write a Python program* to find the maximum and minimum values in a set
```


```python
set_of_numbers={2,3,1,77,3}
set_of_numbers=sorted(set_of_numbers)
print("the Maximum number of set of numbers is",(set_of_numbers[-1])) 
print("the Minimum  number of set of numbers is",(list_of_numbers[0])) 
```

    the Maximum number of set of numbers is 77
    the Minimum  number of set of numbers is 1
    


```python
#**60- Write a Python program that finds all pairs of elements in a list whose sum is equal to a given value.
```


```python

```


```python

```


```python

```


```python

```


```python

```


```python

```


```python

```


```python

```


```python

```


```python

```


```python

```


```python

```


```python

```


```python

```


```python

```


```python

```


```python

```


```python

```


```python

```


```python

```


```python

```


```python

```


```python

```


```python

```


```python

```


```python

```


```python

```


```python

```


```python

```


```python

```


```python

```


```python

```


```python

```


```python

```


```python

```


```python

```


```python

```


```python

```


```python

```


```python

```


```python

```


```python

```


```python

```


```python

```


```python

```


```python

```


```python

```


```python

```


```python

```


```python

```


```python

```


```python

```


```python

```


```python

```


```python

```


```python

```


```python

```


```python

```


```python

```


```python

```


```python

```


```python

```


```python

```


```python

```


```python

```


```python

```
