---
layout: post
title:  "Lecture 1: Installations and first steps"
date:   2017-01-25 16:00:00 +0000
categories: lecture
---

# 1. Installing:

1. Download Python interpreter from [here](https://www.python.org/downloads/release/python-360/). For Windows users select ``Windows x86-64 executable installer``, for Mac pick ``Mac OS X 64-bit/32-bit installer``.
**Please check the box asking you whether you'd like to add python to path.**

2. Secondly, install **Pycharm** from [here](https://www.jetbrains.com/pycharm/download/)
We recommend you install the professional version through your school email, so that you don't have to pay for anything. But if you dont want to register **you can use Comunity Edition** - for our purposes it won't make difference. 

## What are these tools?

Python is a popular programming language and Pycharm is powerful editor for editing Python files.
Think about Pycharm as a sort of Microsoft Word for programming. 

Python intepreter is a program that reads your Python files and tells computer what to do. This is necessary because computers itself work in very primitive programming language called Assembler. So think about this as a middleman between you and computer. 

# 2. Playing with Python

Start Pycharm, it will ask you create a new project. Project in this context means simply a folder that contains your files. You can name it as you want. Then create a new file and put type following  (or copy it from here):

```python
print("Hello world.")
```
Then go to ``Run`` in Toolbar and select to run the file. It should look like this: 

![]({{ site.url }}/assets/l01/hello.png)

Congratulations, you just executed your first computer program.


## Using python as calculator:

Python can be useful as calculator, try these examples: You can just add them to the file.

```python
print(10/2)
print(3.2 * 10212)
print(10 ** 2) # ** is power operator
print(10/2 * 3 + 32 * (11+23))
```


# 3. Python console & Homework

Sometimes you will see people using Python console. This is interactive version of Python - it executes things at the moment. Its useful for experimenting but does not allow you to save your work. You can open in Pycharm by going to ``Tools | Python Console``.

![]({{ site.url }}/assets/l01/console.png)

It might look slightly different in your version of Python. Usually textbooks indicate console by ``>>>`` characters. So when you see something like that you should not copy these. This is what you might see in tutorials and textbooks:

```python
>>> 10+11
21
```

This means that author typed ``10+11`` and the output was ``21``.


## Short homework:

What do these result in:

```python
print('Happy', 30 * 12 * 7 - 503)
```

```python
print("You can join" + "strings together")
```

Strings are the things in ``""`` quotes or ``''`` these quotes. Its quite simply a text. 

```python
print('10' + '12')
print(10 + 12)
```
# 4. Variables:

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

# 5. Basic data types:

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

## I want more:
You can go trough [this tutorial](https://docs.python.org/3/tutorial/introduction.html). It might confuse you. Remember that you can't do anything wrong here - there is no cost to programming so don't worry to experiment. 
