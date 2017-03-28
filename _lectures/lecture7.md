
```python
#discionaries are maps from keys to respective values
#how do you declare diction
czech_engish_words = {
  'slovo': 'word',
  'stul': 'table',
  'slovnik': 'dictionary'
}
#so you have implicit ordering in the dictionary. If you wanted to 


some_list = [1,2,3]
#how do we add an item to a dictionary
czech_engish_words['nevim']='I dont know.'
#if the key was already existing, the new one would overwrite the previously existing one.

#SETS
#We can ask whether certain items belong to these sets or not.

people = {'Monika', 'John', 'Petr'}
uninvited = {'Petr', 'Filip'}
#If you do the line: 'Petr' in people, it gives you out a boolean value of TRUE or FALSE.
people.add('Jirka')
# But Jirka was rude
uninvited.add('Jirka')

#Lists have specific ordering, but not specified keys. If we just want to know if something is in a collection or not, we should use a Set.
#We can do an intersection of two- for example:
#people & uninvited
#gives out 'Jirka' and 'Petr'

#Tuples, the fourth most used data structure. Once you declare them, they stay a certain way. We use them to denote points (for example in geometry). It wouldnt make sense to use a list, because if something went wrong, wouldnt make sense in context of what were doing. A tuple is a value in round brackets, separated by commas. For example...
list_of_coordinates = [
  (30, 11),
  (21, 33)
  ]
for x,y in list_of_coordinates:
    print(x,y)
#or, we could try...
for b in list_of_coordinates:
  print(b[0], b[1])
#the two are, as you can see equivalent. But the first one has a way better notation.
#Make a function that will duplicate values in a list
#Lets start by defining an empty dictionary and an empty function. As you know from previous lectures, to create an empty list you define a certain name equal to an empty set, in case of a list its empty square brackets and for a dictionary it has empty squiggly brackets

vals = {'a', 'b', 'a', 'b']
counter = {}
empty_set = set()
#the function will expect us to include one parameter. 
function_Jirka=0
blbost = [1,2,3,4,5]
  for i in blbost
  function_Jirka = i*2
print (function_Jirka)
print [b]
  
  

# we use if to check if an element is in the dictionary. 
#We use += to add a one to the value

def custom_counter(elems):
  counter = {]
  
```
