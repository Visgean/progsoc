#Lecture 5, Week 7: Functions and revision
So in lecture 5 we mainly revised content from previous lectures and did a couple of exercises, some of which are posted below.
We recommend you to read the questions first, have a go at responding and only when you're done or lost, look at the results. If you struggle, just post your question on the FB group page or chat.
:) Good luck


###Warming up...
Define a function 'some_fun' that for three numbers outputs their product. Then, for three numbers of your choice, print the result with the string 'some_fun' preceding your output.


##Exercise 5.1

Define a function called sum_of_x which contains only numbers which residuals while divided by 2 are zero, i.e. only even numbers.
Hint: In order to define a residual to be equal to zero, use 
```python
i%2 == 0
```
along with if and for statements, where appropriate. Also, do not forget about indentations.


##Exercise 5.2

First define 'numbers' as an empty list. Subsequently, add in all numbers which are divisible by 2 or 3 ranging from 1 to 100. 
Lastly, print the numbers with the string 'multiples of 2 or 3' preceeding your output, which should be a list containing the designated multiples. 


##Exercise 5.3

a) Define a function called maybe_multiply_by_three as one that for values smaller than 5 gives out their exact value and for other, their value multiplied by 3. 
Subsequently test your code by defining x and y as the results of your function for two numbers of your choice (e.g. for 3 and 9) and by testing what values your code outputs.

b) Define a for loop that will give you the output of the function above for all natural numbers from 1 to 15.



##Solutions:

###Warming up...
```python
  
def some_fun(n, x, y):
  return n*x*y
  
print('some_fun', some_fun(3,4,6))
```

###: Exercise 5.1
```python
sum_of_x = 0

for i in range(10000):
  if i%2 == 0:  
    sum_of_x = sum_of_x + i
print(sum_of_x) 
```
###Exercise 5.2
```python
numbers = []
for n in range(100):
  if n % 2 == 0 or n % 3 == 0:
    numbers.append(n)

print('multiples of 2 or 3 ', numbers)
```
###Exercise 5.3 a)
```python
def maybe_multiply_by_three(n):
  if n < 5:
    return n
  return n * 3
  
  print('unreachable')
  
x = maybe_multiply_by_three(3)
y = maybe_multiply_by_three(9)

print(x, y)
```
###Exercise 5.3 b)
```python
for i in range(15):
  print(maybe_multiply_by_three(i))
```
