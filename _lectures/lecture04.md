---
layout: post
title:  "Lecture 3: Functions"
date:   2017-02-15 16:00:00 +0000
categories: lecture
---

# Functions

Functions in Python work similarly to ordinary mathematical ones. They transform the input they're given (in our case it's often strings,in school it might be variable x) and give out an output consisting of results that comply with the criterions we defined in the function.
We can start defining a function as an empty space. Like in the exaple below:
```python
sum_of_x = 0
```
Subsequently, we define a for loop that will, as explained in our last lecture, repeat the subsequent process for
values within the range specified below. 

```python
for i in range(10000):
  if i%2 == 0:  
    sum_of_x = sum_of_x + i
print(sum_of_x) 
```
The condition 'if i%2 == 0' specifies that numbers we are interested in are those, whose remainder after 
a division by two is zero. This means that we are interested in even numbers within the range specifed above.
The next command tells Python to sum all of these (even) numbers cumulatively and to print the sum.

##Exercise 4.1.
Try for yourself: Define a function called ''
