---
layout: post
title:  "Lecture 3: If that then this"
date:   2016-12-01 12:01:08 +0000
categories: lecture
---

# If condition

If conditions are the most basic tool in programming, it allows computer to decide which code gets executed and which blocks to skip.

```python
number_of_apples = 100

if number_of_apples > 5:
    # lets call this block 1
    print("Sir, you have an obscure amount of apples. Are you ok?")
else:
    # lets call this block 2
    print("The number of apples you have is ok. Eat some.")
```

this code decides if block 1 or 2 gets executed based on ``number_of_apples > 5`` condition. If it evaluates to ``True`` block 1 it is. Otherwise block 2. 

You can also ommit the ``else`` statement.

## A little bit of input 

So far we have only dealt with hard-coded values which makes if conditions kind of boring - i mean you already knew what block will get executed. The fun part comes when you plug in the input that you can't predict. This is where the ``input`` function comes in. 


```python
number_of_apples_string = input("Yo, how many apples do you have??? ")
number_of_apples = int(number_of_apples_string)

if number_of_apples > 5:
    print("Sir, you have an obscure amount of apples. Are you ok?")
else:
    print("The number of apples you have is ok. Eat some.")
```

The ``input`` function takes input from user but it does not not know what kind of input you want - it can be any text. But we need a number to compare how many apples we have! Thats where the ``int`` function comes. 

It has its drawbacks: if the user does not provide number but for example string ``none`` your program will crash.



```python 
Yo, how many apples do you have??? I have no fricking apples

Traceback (most recent call last):
  File "apples.py", line 2, in <module>
    number_of_apples = int(number_of_apples_string)
ValueError: invalid literal for int() with base 10: 'I have no fricking apples'
```

This is Python telling you where it crashed and why. Lets go line by line: 


```python 
Traceback (most recent call last):
```

``traceback`` means something like a path that Python followed in your code.  


```python 
File "apples.py", line 2, in <module>
```

This says where exactly did the crash occured. It was in file called ``apples.py`` at the second line.


```python 
number_of_apples = int(number_of_apples_string)
```

this is a line that is responsible for the crash. 


```python 
ValueError: invalid literal for int() with base 10: 'I have no fricking apples'
```

There was an error with value ``int`` requires numbers and you provided ``I have no fricking apples`` a text - not a number. Therefore its ``ValueError``. 



# More ifs

Sometimes you want more ``if`` branches. We call these ``elif``. 

```python
number_of_apples_string = input("Yo, how many apples do you have??? ")
number_of_apples = int(number_of_apples_string)

if number_of_apples < 5:
    print("The number of apples you have is ok. Eat some.")
elif number_of_apples == 11:
	print("What a lovely number of apples!")
elif number_of_apples > 30 and number_of_apples < 40:
	print("You have something like 35 apples. Ok.") 
else:
    print("Sir, you have an obscure amount of apples. Are you ok?")
```

# Practise / homework

Copy the following Python code that calculates the currency conversion and fix it.

```python

USD_PER_GBP = 0.8

money_in_usd = int(input("How many dollars do you have? "))

money_in_gbp = 0 # calculate the correct amount

print('You have {0} brittish pounds'.format(money_in_gbp))


# now fix this condition 

if False: # <- fix this condition
    print("You are GBP milionare.")
else:
    print("poor you")

```

# Reading

1. [Digital ocean tutorial about IFs](https://www.digitalocean.com/community/tutorials/how-to-write-conditional-statements-in-python-3-2)
2. [Official docs](https://docs.python.org/3.6/tutorial/controlflow.html), might be harder to read but goes further.