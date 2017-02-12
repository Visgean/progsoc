---
layout: post
title:  "Lecture 3: For loops"
date:   2017-02-08 16:00:00 +0000
categories: lecture
---

# For loops

For loops' are used to iterate (repeat) a certain function. 

#Example
```
list_of_cubes = [] #we have an empty list
if __name__ == '__main__':
    for element in some_kind_of_list:
        list_of_cubes.append(element * element * element)
        print(list_of_cubes)
        ```
here, we have for every element in the original list we've multiplied it by itself three times and then cumulatively added the products of three elements for each of the elements within the fist list
```
#Example_2
```
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
    
#Example 3 = Range
```
for i in range(5000):
    print(i)
 ```
it's like saying to python : give us first 5000 values starting with zero (including zero)
loops can be infinite. To avoid too much time (e.g. if you had no idea it would be printing unnecessary text), click the button stop on the left side.

# Homework: try for yourself- give us an example of the sum of first 100000 natural numbers
