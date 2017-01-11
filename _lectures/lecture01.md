---
layout: post
title:  "Lecture 1: Installations and first steps"
date:   2016-11-04 12:01:08 +0000
categories: lecture
---

# Installing:

1. Download Python interpreter from [here](https://www.python.org/downloads/release/python-360/). For Windows users select ``Windows x86-64 executable installer``, for Mac pick ``Mac OS X 64-bit/32-bit installer``.
**Please check the box asking you whether you'd like to add python to path.**

2. Secondly, install **Pycharm** from [here](https://www.jetbrains.com/pycharm/download/)
We recommend you install the professional version through your school email, so that you don't have to pay for anything. But if you dont want to register **you can use Comunity Edition** - for our purposes it won't make difference. 

# What are these tools?

Python is a popular programming language and Pycharm is powerful editor for editing Python files.
Think about Pycharm as a sort of Microsoft Word for programming. 

Python intepreter is a program that reads your Python files and tells computer what to do. This is necessary because computers itself work in very primitive programming language called Assembler. So think about this as a middleman between you and computer. 

# Playing with Python

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


# Python console

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


## I want more:
You can go trough [this tutorial](https://docs.python.org/3/tutorial/introduction.html). It might confuse you. Remember that you can't do anything wrong here - there is no cost to programming so don't worry to experiment. 
