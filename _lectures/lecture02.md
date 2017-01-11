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
