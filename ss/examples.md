###Print and Strings

```python
print('Hello World')
```
```python
print("Double quotes")
```
```python
print('concatena'+'tion')
```
```python
print('hello','there')
```
```python
print('I\'m 5')
print("I'm 5")
```

------

###Math

```python
print(1+3)
```
```python
print(1-3)
```
```python
print(1*3)
```
```python
print(1/3)
```
```python
print(1.5/3.6)
```
```python
print(4**2)
```

------

###Variables

```python
exVar = 100
print(exVar)
```
```python
opVar = exVar / 5.3
print(opVar)
```
```python
#Variables cannot start with a number
_100ma = 5
print(_100ma)
```

------

###While Loops

```python
condition = 1

while condition < 10:
    print(condition)
    '''
    multiple
    lines
    can
    go
    here
    '''
    #condition = condition + 1
    condition += 1
```

```python
condition = 5

while condition < 15:
    print('True')
    
while True:
    print('infinite')

```

------

###For Loops

```python
exampleList = [1,6,7,3,6,9,0]

for thing in exampleList
    print(thing)
```

```python
for x in range(1,11):
    print(x)
```

------

###If Statements

```python
x = 2
y = 7
z = 10

if x > y:
    print(x,'is greater than',y)

if x < y:
    print(x,'is less than',y)
    
if x == y:
    print(x,'is the same as',y)

if z > y > x:
    print(z,'is greater than',y,'which is greater than',x)
```

------

###If Else Statements

```python
x = 13
y = 6

if x < y:
    print(x,'is less than',y)
if x > y:
    print(x,'is greater than',y)
else:
    print(x,'is not less than',y)
```

------

###If Elif Statements

```python
x = 3
y = 7
z = 10

if x > y:
    print(x,'is greater than',y)
elif x < z: 
    print(x,'is less than',z)
elif y > z:
    print(y,'is greater than',z)
else: 
    print('nothing was the case')
```

------

###Functions

```python
def example():
    x = 1
    y = 3
    print(x+y)
    
    if x < y:
    print(x,'is less than',y)
    
def main():
    example()
```

------

###Function Parameters

```python
def website(font,background_color,font_size,font_color):
    print('font:',font)
    print('bg:',background_color)
    print('Font size:',font_size)
    print('Font color:',font_color)
    
website('TNR','white','11','black')
```

```python
def website(font='TNR',
            background_color='white',
            font_size=11,
            font_color='black'):
    print('font:',font)
    print('bg:',background_color)
    print('Font size:',font_size)
    print('Font color:',font_color)

website()
```

------

###Global and Local Variables

```python
x = 6

def example():
    z = 5
    print(z)
    
def example2():
    z = 7 
    print(z)
    y = x + 1
    print(y)
    
x = example2()

print(x)
```

------

###Common Python Errors

------

###Writing to a File

------

###Reading From a File

------

###Classes

------

###Input and Statistics

------

###Import Syntax

------

###Making Modules

------

###Error Handling - Try and Accept

------

###Lists vs Tuples and List Manipulation

------

###Dictionaries

------

###Project - Making a Python Program
