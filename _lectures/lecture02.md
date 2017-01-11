---
layout: post
title:  "Lecture 2: Variables and basic types"
date:   2016-11-11 12:01:08 +0000
categories: lecture
---

# Variables:

Variables are one of the most fundamental concept of all programming languagues. They allow us to store and retrieve values. 


```python
>>> name = "Martin"
>>> print(name)
Martin
>>> name = "Pepe"
>>> print(name)
Pepe
```

Math example:

```python
>>> pi = 3.14 # precise enough
>>> r = 10
>>> area = pi * r ** 2
>>> print(area)
314.0
```

You can name your variables however you want. Beginners sometimes stick to using math-like variables ``x``, ``y``. Try to avoid it - its always better to use longer names that convey the meaning of the content of the variable. So instead of ``a`` use ``area``.

Name requirements:
 - variables can't start with numbers - ``1apple`` is invalid while ``apple1`` is valid. 
 - you can use undescores but not dots or ``-`` signs. So ``speed_of_light`` is valid while ``speed-of-light`` and ``speed.of.light`` are both invalid.
 - names are case sensitive ``Speedoflight`` and ``speedoflight`` are two different variables!

# Basic data types:

What are types? They are representation of different values - in real world you have many types of objects - numbers, cars, devices, pigment types, genders... In computer science they more precisely defined, this is to ensure that computer undestand the meaing of the value. 

```python
>>> integer = 1 # whole number
>>> floating_number = 1.3
>>> text_variable = "Lorem ipsum"
>>> boolean = True
```

One of the reason for variables is to ensure that the behaviour for operators is clearly defined. For example we can't add text with numbers - that simply does not make sense! And so Python will throw an exception (signaling undefined behaviour):

```python
>>> text_variable + integer
Traceback (most recent call last):
  File "<stdin>", line 1, in <module>
TypeError: Can't convert 'int' object to str implicitly
```
This is just python special way of telling you that you did something wrong. Just like you can't add apples and pears together you can't add two different types together. 

Imagine this situation: ``1 + '2'`` what should the result of this operation be? Should it be string? Or integer? Who knows? Python does not so it throws an tantrum.


## Lists

Lists are Python way of storing mulitple values in an array. 

```python
>>> fruits = ["bananas", "apples", "oranges", "melones"]
>>> numbers = [1,2,3,4,5,11,-1]
>>> mixed = [1,2,3, "bananas"]
```

Lists are defined by square brackets, and comma separated values. Usually it makes sense to store values of same type (``mixed`` in example above shows that it is not required though). 

You can add stuff to lists using ``.append`` method:

```python
>>> fruits
['bananas', 'apples', 'oranges', 'melones']
>>> fruits.append("potato")
>>> fruits
['bananas', 'apples', 'oranges', 'melones', 'potato']
```

or you can extend the list by another list:

```python
>>> fruits
['bananas', 'apples', 'oranges', 'melones', 'potato']
>>> fruits.extend(numbers)
>>> fruits
['bananas', 'apples', 'oranges', 'melones', 'potato', 1, 2, 3, 4, 5, 11, -1]
```

you can then select a single element - where 0 denotes first element.

```python
>>> fruits
['bananas', 'apples', 'oranges', 'melones', 'potato', 1, 2, 3, 4, 5, 11, -1]
>>> fruits[0]
'bananas'
>>> fruits[1]
'apples'
>>> fruits[3]
'melones'
```

or you can get a range of elements - this is called slicing:

```python
>>> fruits[0:2]
['bananas', 'apples']
>>> fruits[1:4]
['apples', 'oranges', 'melones']
>>> fruits[:3]
['bananas', 'apples', 'oranges']
>>> fruits[1:]
['apples', 'oranges', 'melones', 'potato', 1, 2, 3, 4, 5, 11, -1]
>>> fruits[3:]
['melones', 'potato', 1, 2, 3, 4, 5, 11, -1]
```

# Nesting
One of the many recurring themes of programming is nesting: list can contain lists. So here is is list containing a list containing a list containing a list... You get the point

```python
nested = [[[[[[[[[[[[[[[[[[[[[[[[[  'Base level'  ]]]]]]]]]]]]]]]]]]]]]]]]]
```

to retrieve this element you need to retrieve the first (and only) element of the nested. And then its first (and only) element... And so on. 

```python
>>> nested[0][0][0][0][0][0][0][0][0][0][0][0][0][0][0][0][0][0][0][0][0][0][0][0][0]
'Base level'

```


# I want MORE! (Reading)
- [This tutorial](https://www.programiz.com/python-programming/list) is a good comphrenensive resource.
- [Dive into Python](http://www.diveintopython3.net/native-datatypes.html) is an excelent resource. Again, don't worry if you don't understand everything. 