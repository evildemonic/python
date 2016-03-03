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

```python
#NameError: name 'varaible' is not defined
variable = 55
print(varaible) #mispelled
```

```python
#Expected Indented Block
def func1():

def func2():
    print(2)
```

```python
#Unexpected Indent
def task():
    print('1')
    
print('2')

    print('3')
```

```python
#Didn't close string / EOL while scanning string literal

print('Hey there how are you today?
```

```python
#Didn't close print statement / unexpected EOF while parsing

print('Hey there how are you today?'
```
------

###Writing to a File

```python
#Will completely overwrite an existing file
writeMe = 'Example text'

saveFile = open('exampleWrite.txt','w') # 'w' = write
saveFile.write(writeMe)
saveFile.close()
```

------

###Appending to a File

```python
#Appends an existing file; creates one if it doesn't exist
appendMe = 'Some text'

saveFile = open('exampleFile.txt','a') # 'a' = append
saveFile.write('\n') # \t tab, \s space, \n new line 
saveFile.write(appendMe)
saveFile.close()
```

------

###Reading From a File

```python
readMe = open('exampleFile.txt','r') # 'r' = Read
print(readMe)
```
```python
splitMe = readMe.split('\n)
print(splitMe[2])
```
```python
readme2 = open('exampleFile.txt','r').readlines()
print(readMe2)
```

------

###Classes

```python
class calc: 
    
    def add(x,y):
        answer = x + y
        print(answer)
    def sub(x,y):
        answer = x - y
        print(answer)
    def mult(x,y):
        answer = x * y
        print(answer)
    def div(x,y):
        answer = x / y
        print(answer)

calc.add(5,3)
calc.mult(5,3)
calc.div(5/3)
calc.sub(5-3)
```

------

###Input and Statistics

```python
name = input('What is your name?: ')
print('Hello',name)
```

```python
import statistics

exList = [5,3,2,9,9,7,4,3,1,8,9]

x = statistics.mean(exList)
print(x)

x = statistics.median(exList)
print(x)

x = statistics.mode(exList)
print(x)

x = statistics.stdev(exList)
print(x)

x = statistics.variance(exList)
print(x)
```

------

###Import Syntax

```python
import statistics

exList = [5,6,2,1,6,7,2,2,7,3,7,7,7]

print(statistics.mean(exList))
```
```python
import statistics as s

exList = [5,6,2,1,6,7,2,2,7,3,7,7,7]

print(s.mean(exList))
```
```python
from statistics import mean

exList = [5,6,2,1,6,7,2,2,7,3,7,7,7]

print(mean(exList))
```
```python
from statistics import mean as m

exList = [5,6,2,1,6,7,2,2,7,3,7,7,7]

print(m(exList))
```
```python
from statistics import mean, stdev

exList = [5,6,2,1,6,7,2,2,7,3,7,7,7]

print(mean(exList))
print(stdev(exList))
```
```python
from statistics import mean as m, stdev as s

exList = [5,6,2,1,6,7,2,2,7,3,7,7,7]

print(m(exList))
print(s(exList))
```
```python
from statistics import * #imports everything

print(mean(exList))
print(stdev(exList)) #, etc
```
------

###Making Modules

```python
def exampleFunct(data):
    print(data)
    
# >>> exampleFunc('this is a test')
```

```python
import exampleModule

exampleModule.exampleFunct('test')
```

------

###Error Handling - Try and Except

```python
#Can't convert 'int' object to str implicitly
try:
    print('Running the try...')
    print('5'+5)
    
except Exception as e:
    print(str(e))
```
```python
try:
    print('Running the try...')
    print('5'+5) #or ('5'+x) for second except
    
#for TypeError
except TypeError as t:
    print('TypeError triggered')
    
#for NameError
except NameError as n:
    print('NameError triggered')
    
#for any other errors
except Exception as e:
    print('General Exception')
```

------

###Lists vs Tuples and List Manipulation

```python
#Tuple; immutable
def example():
    return 15,19
    
a,b = example()

print(a)
print(b)
```
```python
#List; mutable
x = [6,2,3,6,8,9,4,3]

print(x)
print(x[5])

x.append(12) # adds 12 to the end of the list
print(x)

x.insert(5,7) # inserts 7 at the 5th position
print(x) 

x.remove(7) # removes the first 7
print(x)

print(x.index(12)) # what position a number is in

print(x.count(3)) # number of times something is in the list
```
```python
x = ['Spot','Cam','Jan','Dave','Zack']

print(x)
x.sort() # Alphebetizes list
print(x)

x.reverse() # Reverses List Order
print(x)
```

------

###Dictionaries

```python
gradeDict = {'Kelly':89, 'David':65, 'Jack':95, 'Samantha':78}

print(gradeDict)

print(gradeDict['David'])

gradeDict['David'] = 56

gradeDict['Jessy'] = 92

print(gradeDict)

del gradeDict['David']

print(gradeDict)
```
```python
gradeDict = {'Kelly':[89,88],
             'Jack':[95,87], 
             'Samantha':[78,89], 
             'Jessy':[92,99]}
             
print(gradeDict)

print(gradeDict['Jessy'])

print(gradeDict['Jessy'][0])
```
------

###Project - Making a Python Program
