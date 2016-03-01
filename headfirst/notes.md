###Head First Python Notes 
======


#####Lists

```
movies = ["The Holy Grail", "The Life of Brian", "The Meaning of Life"]
```

To print out items in the list: 

```
print(movies[#]) # 0, 1, 2, 3...
```
(Python starts counting from 0.)

**To count the number of items in a list:**
(len)
```
print(len(variable))
```
variable = the set variable, like "movies" above; example: print(len(movies))

```
cast = ["Cleese", "Palin", "Jones", "Idle"]
print(cast)
```
['Cleese', 'Palin', 'Jones', 'Idle']

```
print(len(cast))
```
4

```
print(cast[1])
```
Palin

**Editing a list:**

Add a single data item to the end of the list with **append()**; remove data from the end of the list with **pop()**, and add multiple items to the list with **extend()**.

```
cast.append("Gilliam")
print(cast)
```
['Cleese', 'Palin', 'Jones', 'Idle', 'Gilliam']

```
cast.pop()
```
'Gilliam'

```
print(cast) 
```
['Cleese', 'Palin', 'Jones', 'Idle'] 

```
cast.extend(["Gilliam", "Chapman"]) 
print(cast)
```
['Cleese', 'Palin', 'Jones', 'Idle', 'Gilliam', 'Chapman']

**Remove a specific item from a list with remove(); add an item to a specific location with insert().**

```
cast.remove("Chapman")
print(cast) 
```
['Cleese', 'Palin', 'Jones', 'Idle', 'Gilliam']
```
cast.insert(0, "Chapman")
print(cast) 
```
['Chapman', 'Cleese', 'Palin', 'Jones', 'Idle', 'Gilliam']
