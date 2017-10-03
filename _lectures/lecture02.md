---
layout: post
title:  "Lecture 2 - Functions"
date:   2017-09-28 17:00:00 +0000
categories: lecture
---


# Lecture 2, Week 2: Functions

Functions are useful ‘tools’ that take an input and give you an output depending on the rule you defined for it. 
You learnt to do something similar with IF conditions or FOR loops where you defined what should be done with which variables and how.
Functions can enhance your program because you can more easily reuse them throughout the program 
without having to define it again and again. You only need to provide a new input. 
It also makes the program more modular – more decomposable into parts.

##  How to create a function


### Step 1. Define your function

Python will always know you are about to specify a function if you write 


```python
def
```

followed by a space, name of the function and brackets that include chosen number of arbitrary letters of words, which are called the arguments, and finish up with a colon. 

Example:
```python
def my_addition(x, y):
```
You might wonder what x and y are. 
They are some arbitrary symbols and Python will understand that they represent the general form of the input you will be giving them. 
In this case, your function will require you to provide 2 inputs. 

### Step 2. Tell Python the general form of your function 

Now that Python knows you are meaning to create a function it will expect you to tell it what the function should be doing. 
A function can be super basic as well as super complex. At the end of the function you write
```python
return
```
after which you specify the operation that should be done to the input so that it can return some output.
 
A simple example can be:

```python
print('The sum of', x, 'and', y, 'equals to')
return x+y

```
NOTE: Remember to indent (=leave spaces in front) whatever lines belong within the function
So the entire function looks like this:
```python
def my_addition(x, y):
   print('The sum of', x, 'and', y, 'equals to')
   return x+y
```
### Step 3. Calling a function

Now that you have a general formula for you function, you can input items into it to receive some output. 
You call a function with print to actually see the output printed.
```python
print(my_addition(30, 25))
```
You should see this happen:

#### The sum of 30 and 25 equals to 55

And you can then change the values of your two arguments to any number and call it again and again 
without having to touch the structure of your function.

##  TASK 1

Create a function in which you can input three arguments: 
1. your budget for the month
2. the rent you have to pay monthly
3. the price of a kg of potatoes

and let output the maximum kg of potatoes you can consume in a given month.

##  TASK 2

Create a max function with 2 arguments. This basically means a function that will take as an input 2 variables and will return the bigger on. Call it my_max. (Hint: Use your skills from previous lessons.)


##  TASK 3

Look at this recursive function below and try to guess what it does. Try to run it to see what happens. 

def fib(n):
  if n == 0:
    return 1
  if n == 1:
    return 1
  return fib(n-1) + fib(n-2)
  
print('Fib of 10:', fib(10))

### NOTE: Try these inputs:
a) 10
b) 100
c) 1 000

### Explanation:

The function above illustrates the Fibonacci sequence; 
the argument n specified which term of the sequence we were looking for and the output was the nth term in the sequence.

As we learnt in the lesson, 
it can take a while for Python to give you the answer because it will keep iterating and performing the operation over and over again 
for all n’s from the beginning term until it reaches let’s say n = 1 000 (so 1000 iterations).
As it doesn’t save it’s results in the meantime. 
We also tried in the lesson to then integrate a list or a dictionary in the function, 
that was saving the results the program was running, which increased the speed of the program. 
However, it could sometimes be easier to use a simple For loop, which we’ve done in the previous lesson. 


