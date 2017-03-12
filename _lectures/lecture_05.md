#Lecture 5, Week 7: Functions and revision
So in lecture 5 we mainly revised content from previous lectures and did a couple of exercises, some of which are posted below.
We recommend you to read the questions first, have a go at responding and only when you're done or lost, look at the results. If you struggle, just post your question on the FB group page or chat.
:) Good luck

##Exercise 5.1

Define a function called sum_of_x which contains only numbers which residuals while divided by 2 are zero, i.e. only even numbers.
Hint: In order to define a residual to be equal to zero, use 
```python
i%2 == 0
```
along with if and for statements, where appropriate. Also, do not forget about indentations.

##Exercise 5.2












##Solutions:
###: Exercise 5.1
```python
sum_of_x = 0

for i in range(10000):
  if i%2 == 0:  
    sum_of_x = sum_of_x + i
print(sum_of_x)  
  
numbers = []
for n in range(100):
  if n % 2 == 0 or n % 3 == 0:
    numbers.append(n)

print('multiples of 2 or 3 ', numbers)
```

