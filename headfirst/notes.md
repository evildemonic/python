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

**To insert data INTO an existing item on a list:**

```python
movies.insert(1, 1975)

movies.insert(3, 1979)

movies.append(1983)
```

```python
movies = ["The Holy Grail", 1975, "The Life of Brian", 1979, "The Meaning of Life", 1983]
```

```python
fav_movies = ["The Holy Grail", "The Life of Brian"]

print(fav_movies[0])
print(fav_movies[1])
```
To continue the above code, use a **for** loop:

```python
fav_movies = ["The Holy Grail", "The Life of Brian"]

for each_flick in fav_movies: 
    print (each_flick)
```


