###Head First Python Notes 
======


#####Lists

```python
movies = ["The Holy Grail", "The Life of Brian", "The Meaning of Life"]
```

To print out items in the list: 

```python
print(movies[#]) # 0, 1, 2, 3...
```
(Python starts counting from 0.)

**To count the number of items in a list:**
(len)
```python
print(len(variable))
```
variable = the set variable, like "movies" above; example: print(len(movies))

```python
cast = ["Cleese", "Palin", "Jones", "Idle"]
print(cast)
```
['Cleese', 'Palin', 'Jones', 'Idle']

```python
print(len(cast))
```
4

```python
print(cast[1])
```
Palin

**Editing a list:**

Add a single data item to the end of the list with **append()**; remove data from the end of the list with **pop()**, and add multiple items to the list with **extend()**.

```python
cast.append("Gilliam")
print(cast)
```
['Cleese', 'Palin', 'Jones', 'Idle', 'Gilliam']

```python
cast.pop()
```
'Gilliam'

```python
print(cast) 
```
['Cleese', 'Palin', 'Jones', 'Idle'] 

```python
cast.extend(["Gilliam", "Chapman"]) 
print(cast)
```
['Cleese', 'Palin', 'Jones', 'Idle', 'Gilliam', 'Chapman']

**Remove a specific item from a list with remove(); add an item to a specific location with insert().**

```python
cast.remove("Chapman")
print(cast) 
```
['Cleese', 'Palin', 'Jones', 'Idle', 'Gilliam']
```python
cast.insert(0, "Chapman")
print(cast) 
```
['Chapman', 'Cleese', 'Palin', 'Jones', 'Idle', 'Gilliam']
