# Homework

##  Q1

Define a function called sum_of_x which contains only numbers which residuals while divided by 2 are zero, i.e. only even numbers.
Hint: In order to define a residual to be equal to zero, use 

```python
i%2 == 0
```
along with if and for statements, where appropriate. Also, do not forget about indentations.

### Solution

```python
sum_of_x = 0

for i in range(10000):
  if i%2 == 0:  
    sum_of_x = sum_of_x + i
print(sum_of_x) 
```

##  Q2
First define 'numbers' as an empty list. Subsequently, add in all numbers which are divisible by 2 or 3 ranging from 1 to 100. 
Lastly, print the numbers with the string 'multiples of 2 or 3' preceeding your output, which should be a list containing the designated multiples. 

### Solution

```python
numbers = []
for n in range(100):
  if n % 2 == 0 or n % 3 == 0:
    numbers.append(n)

print('multiples of 2 or 3 ', numbers)
```

## Q3
Run a for loop stored in the list called 'my_contacts' for the dictionary called 'phonebook' (you can copy it above),
so that 'my_contacts' includes strings in the form e.g. 'Peter has the number 123456.

### Solution
https://www.w3resource.com/python-exercises/dictionary/python-data-type-dictionary-exercise-5.php
