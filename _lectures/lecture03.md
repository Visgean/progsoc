---
layout: post
title:  "Lecture 3: For loops"
date:   2017-02-08 16:00:00 +0000
categories: lecture
---

# For loops

For loops' are used to iterate (repeat) a certain function. 

#Example

```python
list_of_cubes = [] #we have an empty list
if __name__ == '__main__':
    for element in some_kind_of_list:
        list_of_cubes.append(element * element * element)
        print(list_of_cubes)
```
here, we have for every element in the original list we've multiplied it by itself three times and then cumulatively added the products of three elements for each of the elements within the fist list.
Loops can be infinite. To avoid too much time spent waiting for one
(e.g. if you had no idea it would be printing unnecessary text), click the button stop on the left side.

#Example_2

```python
new_filtered_list = []
big_elements = []
for element in some_kind_of_list:
    if element <= 4:
        new_filtered_list.append(element)
    else:
        big_elements.append(element)

print(new_filtered_list)
print(big_elements)
   ```
    
#Example_3 - Range

```python
for i in range(5000):
    print(i)
```
 
Using Range function in this case is like saying to Python : give us first 5000 values starting with zero (including zero).
Range can be defined either as values leading up to a certain integer (as seen above), mind you that zero is 
seen as the first number, or as a range across values.
e.g.

```python
for i in range(3, 15):
    print(i)
```
This example would give you only the values in the designated interval. Adding more values between 3 and 15
will not change the outcome. Python won't however work with more than 3 values defining a range of numbers.


# Homework
try for yourself- give us an example of the sum of first 100000 natural numbers
