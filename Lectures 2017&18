---
layout: post
title:  "Lecture 1: For loops, range and dictionaries"
date:   2017-09-21 17:00:00 +0000
categories: lecture
---


# Lecture 1, Week 1: For loops, range and dictionaries

##	For Loops

We use for loops to iterate over a given sequence. Let’s consider the following example:
We have a list of prime numbers from two to seven, called primes. For now, let’s write a for loop that returns each number included in primes. 

```python
primes = [2, 3, 5, 7]
for prime in primes:
	print(prime)
```
*The way we address each member is up to you. You can call them primes, x, n, whichever other word. Just remember to avoid pre-defined words used by Python and be consistent*

Also, notice the indentation of the code. Print is tightly linked with the line above it. That is why we indent it. 

•	Let’s try something a bit more elaborate. It’s great that we’ve managed to get the list of all the primes we’ve defined. What if, however, we wanted to change each term of a list? We might find that defining a new list that can store the output of such a change may be a good idea.
```python
first_10_ns = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10]
sum_holder = 0
```

This time, we’ve defined a list of first ten integers as first_10_ns (for some reason starting with a 1). We also defined sum_holder as an empty list for now. It is so that when we alter members of first_10_ns, we have a place where to store them.

```python
for n in range(11):                    #as you can see, n here means nth member of the list
sum_holder = sum_holder + n	#here we’re saying that for each nth term, we add the previous value(s) to the number, so that values compile. 
print('Sum holder:', sum_holder, 'n:', n)	#And finally this line gives out the results, with strings ‘Sum holder:’ and ‘n:’ added for better clarity. Also, notice the comma separating the two kinds of values that are being printed by the function.

print('total:', sum_holder)
```



##Range()

Range() is a pre-defined function which generates a list of numbers we usually iterate over with for loops. It’s best explained with an example
```python
for i in range(5):
	print(i)
```
-this gives out the first integers up to 5. And yes, 0 is the first one. 

We can have range pick out just a certain interval of values.
```python
for i in range(3, 6):
	print(i)
```
As can be seen above, if we define range for a specific interval, we get the parameters 
Between the two numbers, including the lower one (3 in this case), strictly up to the upper bound.

**Extra info** 
Range can, however, take in even three parameters. Let’s try:
```python
for i in range(3, 16, 3)
	print i
```
Here, we see that the lines above give out every third number from 3 to 16.


##Dictionaries

Dictionaries are used in Python similarly like those you know from real life. The attribute specific values to specific keys. The syntax of dictionaries is a bit more tricky than we’ve been used to this far. Important things to note are:

1.	Each key is separated from its value by a colon
2.	The items are separated by commas
3.	And the whole thing is enclosed in curly brackets. (An empty dictionary: {})
4.	Each key (first in the dictionary) is unique, but values aren’t. 

In the end, a dictionary may look like this: 
```python
simple_dictionary_cz_en = {
  'Ahoj': 'Hello',
  'Nenavidim te': 'I love you',
}
```
Here we see that ‘Ahoj’ and ‘Nenavidim te’ are keys, each with a respective value added to it. If you’re confused as to why are the pair below each other, it’s just for the sake of it being neat. The important thing is, however, that each pair is separated by a comma and that the entire dictionary is framed by curly brackets, as specified above.

So if you’d like to get the translation of what Ahoj means in English, you can go about it by writing:

print(simple_dictionary_cz_en['Ahoj'])
 
***Let’s look at other examples:
```python
some_other_dict = {
  1: 3,
  3: 'no types here...'
}

person = {
  'age' : 25,
  'name': 'John'
}
```
As you can see above, some_other_dict and person are two dictionaries which have both strings and numbers for values. This is because values in dictionaries are, unlike keys, mutable. This means that whilst it is OK for values to be either strings, numbers or tuples, keys must be consistent in whether they are either of the three.

*** Now let’s take the example of a phonebook, which, just like a dictionary, attributes each key (name) a value (number). 
```python
phonebook = {
  "Peter": 123456,
  "Jenny": 564684,
  "Kate": 354897
}
```
What to do with such a dictionary next? Imagine having a real virtual phonebook and wanting to check whether your friend’s number to call him. If you had a hard copy, it could take you some time. If the phonebook was virtual, however, you could find his number quite easily- and here is how:

We are going to apply functions if and else we learned last time. We start by user_specified_name, i.e. the name of your friend.

User_specified_name = input(‘Please input a name:’)

**We have defined user_specified_name to ask for the name of the designated person through the function input(). Input stops the program flow, until the user has given his input and ended his input with a return key. It also has an optional parameter-a string- which in our case says ‘Please input a name:’. It is there mostly so that the user knows what is required of him and whilst it is not mandatory to include a string telling one what to do, it may prove to be rather efficient.

```python             
for key,value in some_other_dict.items():
  print("key", key, "value", value)
  ```

It is worth mentioning here, that key and value are not words pre-defined in Python 3. 
Hence you can use unkowns to represent keys and values and don’t have to resort to the labels we used here. Just bear in mind that it is of essence to be consistent with labels.

So there you have it. We recommend you take a bit of a break now to soak all the information in and try and copy the code above, modify it, create your own versions and when you’re done, please attempt the homework we’ve got for you. 

We also recommend you visit the sites listed below for further reference.

