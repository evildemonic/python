
##Unit 1: How to get started: your first program

####Introducing the Web Crawler
A web crawler is a program that collects content from the web. A web crawler finds web pages by starting from a seed page and following links to find other pages, and following links from the other pages it finds, and continuing to follow links until it has found many web pages.

Here is the process that a web crawler follows:

* Start from one preselected page. We call the starting page the "seed" page.
* Extract all the links on that page. (This is the part we will work on in this unit and Unit 2.)
* Follow each of those links to find new pages.
* Extract all the links from all of the new pages found.
* Follow each of those links to find new pages.
* Extract all the links from all of the new pages found.
* ...

This keeps going as long as there are new pages to find, or until it is stopped.

In this unit you will be writing a program to extract the first link from a given web page. In Unit 2, you will find out how to extract all the links on a web page. In Unit 3, you will see how to keep the crawl going over many pages.

======

####Quiz 1: First Quiz
What is the goal of Unit 1 ?

* a. Get started programming.
* b. Learn important computers science concepts.
* c. Write code to extract a link from a web page.
* d. Write code to rank web pages.
 
**Answer:** (a), (b), & (c)

======

###Programming 

**Programming** is the core of computer science.

A **computer** is a machine that can execute a program. With the right program, a computer can do any mechanical computation you can imagine.

A **program** describes a very precise sequence of steps. Since the computer is just a machine, the program must give the steps in a way that can be executed mechanically. That is, the program can be followed without any thought.

A **programming language** is a language designed for producing computer programs. A good programming language makes it easy for humans to read and write programs that can be executed by a computer.

**Python** is a programming language. The programs that we write in the Python language will be the input to the Python interpreter, which is a program that runs on the computer. The Python interpreter reads our programs and executes them by following the rules of the Python language.

======

###Quiz 2: What is a Programming Language

What is a programming language?

* a. a language designed to be executed by computers
* b. a language designed for describing programs
* c. a language designed to be written by humans, and executed by computers
* d. a language designed to be read by humans, and written by computers
* e. a language designed to be read and written by humans, and executed by computers

**Answer:** (a), (b), (c), (d), & (e)

======

###Getting Started with Python Programming

We have provided a way for you to run Python programs using your web browser. You do not need to install any extra programs to do this.

There are two parts to the Python programming environment you will see in your web browser:

 1. The top part is an editor, where you can write and edit code.
 2. The bottom part is an output window, where you can see the results of running your code.

To try running your code, click the "Run" button below the editor.

![image](http://i.imgur.com/1PMUL2R.png)

Find the value of something in Python by using print like this:

```
print 3
3
```
Use a Python expression to return a value. Here are some examples:
```
1 + 1   #addition
2 - 1   #subtraction
2 * 6   #multiplication
```
You can compose expressions to make more complicated expressions, such as:
```
52 * 3 + 12 * 9
```
You can also use parentheses to group expressions:
```
(52 * 3) + (12 * 9)
```
which is different from:
```
52 * (3 + 12) * 9
```
The code below prints out the number of seconds in a year:
```
print 365 * 24 * 60 * 60
31536000
```
======

###Quiz 3: First Programming Quiz

Write a Python program that prints out the number of minutes in seven weeks. You should enter your program in the editor window (top part), and then click "'Run'" to see the output in the bottom part.

```
# This is a Python comment. Lines that begin with a '#' are ignored by the
# Python interpreter. Comments are useful for documenting code or explaining
# quiz questions!
# 
# Write a Python program that prints out the number of minutes in seven weeks.
# Remember: 7 weeks 7 days in a week, 24 hours in a day, and 60 mins in an hour.
# Multiplying these numbers together will give you the result
#
# Click the "Test Run" button below to try running your code and see the output,
# and click "Submit" to submit your answer.

print 7 * 7 * 24 * 60
```
======

###Would You Rather
Why should you learn new languages, like Python, to program computers, rather than using natural languages like English or Mandarin?

There are many reasons why a designed language like Python is better for writing programs than a natural language like English. One problem with natural languages is that they are ambiguous. Hence, not everyone will interpret the same phrase the same way. To program computers, it is important that we know exactly what our programs mean, and that the computer will run them with the meaning we intended. Another problem with natural language is that they are very verbose. To say something with the level of precision needed for a computer to be able to follow it mechanically would require an awful lot of writing. You want your programs to be short so it is less work to write them, and so that it is easier to read and understand them.

======

###Grammar
Compared to a natural language, programming languages adhere to a strict grammatical structure. In English, even if a phrase is written or spoken incorrectly, it can still be understood with the help of context or other cues. On the other hand, in a programming language like Python, the code must match the language grammar exactly. The Python interpreter has no idea what to do with input that is not in the Python language, so it produces an error.

**Basic English Grammar Rules:**

Sentence → Subject Verb Object

Subject → Noun

Object → Noun

Verb → **Eat**

Verb → **Like**

Noun → **I**

Noun → **Python**

Noun → **Cookies**

When programming language grammar is not followed the interpreter will return a SyntaxError message. This means that the structure of the code is inconsistent with the rules of the programming language.

======

###Backus-Naur Form

The notation we used to describe the grammar is known as Backus-Naur Form, which was introduced in the 1950s by John Backus, the lead designer of the Fortran programming language at IBM.

The purpose of Backus-Naur Form is to describe a programming language in a simple and concise manner. The structure of this form is:

```
<Non-Terminal> → replacement
```

The replacement can be any sequence of zero or more non-terminals or terminals.

Terminals never appear on the left side of a rule. Once you get to a terminal there is nothing else you can replace it with. Here is an example showing how to derive a sentence by following the replacement rules:

![image](http://i.imgur.com/UcvRhJ3.png)

Sentence → Subject Verb Object

→ Noun Verb Object

→ **I** Verb Object

→ **I Like** Object

→ **I Like** Noun

→ **I Like Python**

The important thing about a replacement grammar is that we can describe an infinitely large language with a small set of precise rules.

======

###Quiz 4: Eat Quiz

Which of these sentences can be produced from this grammar, starting from sentence?

a. Python Eat Cookies
b. Python Eat Python
c. I Like Eat

**Answer:** (a) & (b)

======

###Python Expressions

An **expression** is something that has a value. Here are some examples of expressions in Python:

```
3
1 + 1
7 * 7 * 24 * 60
```
Here is one of the rules of the Python grammar for making expressions:

Expression → Expression Operator Expression

The Expression non-terminal that appears on the left side can be replaced by an Expression, followed by an Operator, followed by another Expression. For example, 1 + 1 is an Expression Operator Expression.

The interesting thing about this rule is that it has Expression on both the left and right sides! This looks circular, and would be, except we also have other rules for Expression that do not include Expression on the right side. This is an example of a **recursive definition**. To make a good recursive definition you need at least two rules:

1. A rule that defines something in terms of itself.
Expression → Expression Operator Expression

2. A rule that defines that thing in terms of something else that we already know.
Expression → Number

Recursive definitions are a very powerful idea in computer science. They allow us to define infinitely many things using a few simple rules. You will see this more in Unit 6.

Here are some of the Python grammar rules for arithmetic expressions:

* Expression → Expression Operator Expression
* Expression → Number
* Operator → **+**
* Operator → *****
* Number → **0, 1, ...***


Here is an example derivation using this grammar:

* Expression → Expression Operator Expression
* → Expression + Expression
* → Expression + Number
* → Expression **+ 1**
* → Expression Operator Expression **+ 1**
* → Number Operator Expression **+ 1**
* → 2 Operator Expression **+ 1**
* → 2 * Expression **+ 1**
* → 2 * Expression Operator Expression **+ 1**
* → 2 * Number Operator Expression **+ 1**
* → 2 * 3 Operator Expression **+ 1**
* → 2 * 3 * Expression **+ 1**
* → 2 * 3 * Number **+ 1**
* → **2 * 3 * 3 + 1**
* (Note: the example here is slightly different than the one in the video. The 3+3 expression has been changed to 3*3, since the precedence rules in Python would have grouped 2 * 3 + 3 + 1 as (2 * 3) + 3 + 1, so it would not be interpreted as shown in the derivation.)

We need to add one more rule to our expression grammar to be able to produce all of the expressions we have used so far:

* Expression → (Expression)
 
======

###Quiz 5: Python Expressions

Which of the following are valid Python expressions that can be produced starting from Expression? There may be more than one.

a. 3
b. ((3)
c. (1 * (2 * (3 * 4)))
d. + 3 3
e. (((7)))

**Answer:** (a), (c), & (e)

======

###Quiz 6: Speed of Light

Write Python code to print out how far light travels in centimeters after one nanosecond using the multiplication operator.

* The speed of light is 299792458 meters per second.
* One meter is 100 centimeters.
* One nanosecond is one billionth (1/1000000000) of a second.

The reason for computing this is because the distance light travels in a nanosecond really matters in computing! A typical computer today executes billions of steps every second. The processor I am using is a 2.7 GHz processor. The GHz means gigahertz which is a billion cycles per second. So, the computer executes 2700000000 cycles per second.

You can think of each cycle as executing a very small instruction step. If you are using a Mac, you can see how fast your processor is by selecting the Apple menu and choosing About this Mac. If you are using a Windows 7 machine, open the Control Panel and select System and Security, then under System select View amount of RAM and processor speed.

We can compute how far light travels in the time it takes for the computer to complete one cycle:
```
print 299792458 * 100 * 1.0/1000000000 *1/2.7
11.1034243704
```
This is approximately 3/4 of the length of a dollar bill.
![image](http://i.imgur.com/PEVNpYb.png)

A **processor** is the part of the computer that carries out the steps specified in a computer program. Sometimes people call the processor the "central processing unit" or CPU.

A processor has to be small to execute programs quickly. If your computer's processor were any larger than the size of a dollar bill, then you couldn't even send light from one end of the processor to the other before finishing the execution of a single step in a program.

**Answer:** 

```
# Write Python code to print out how far light travels 
# in centimeters in one nanosecond.  Use the values
# defined below.    
# speed_of_light = 299792458   meters per second
# centimeters = 100            one meter is 100 centimeters
# nanosecond = 1.0/1000000000  one billionth of a second
print 299792458 * 100 * 1.0/1000000000
```
======

###Admiral Grace Hopper (1906- 1992)
Grace Hopper was a pioneer in computing who was known for walking around with nanosticks. Nanosticks are pieces of wire that are the length light travels in a nanosecond, about 30 cm.

Hopper wrote one of the first programming languages, COBOL, which was for a long time the world's most widely used programming language. Hopper built the first compiler. A compiler is a program that takes as input a program in a programming language easy for humans to write and outputs a program in another language that is easier for computers to execute. The difference between a compiler and an interpreter like Python is that a compiler does all the work at once and creates a new program, whereas, the interpreter converts the source code one step at a time as the program runs.

When Grace Hopper started building the first compiler, most people did not believe it was possible for a computer program to produce other computer programs: "Nobody believed that I had a running compiler and nobody would touch it. They told me computers could only do arithmetic."

======

###Variables
A **variable** is a name that refers to a value. In Python, we can use any sequence of letters and numbers and underscores (_)when we want to make a variable name, so long as it does not start with a number. Here are some examples of valid variable names:
```
processor_speed
n
Dorina
item73
```
To introduce a new variable, we use an assignment statement:
* Name = Expression
After executing an assignment expression, the name refers to the value of the expression on the right side of the assignment:
```
speed_of_light = 299792458
```
We can use the variable name anywhere we want and it means the same things as the value it refers to. Here is an expression using the name to print out the speed of light in centimeters/sec:
```
print speed_of_light * 100
```
You can create new variables to keep track of values in programs. Here is an expression to find the length of the nanostick in centimeters:
```
speed_of_light = 299792458
billionth = 1.0 / 1000000000
nanostick = speed_of_light * billionth * 100
print nanostick
```
======
###Quiz 7: Variables
Given the variables defined below, write Python code that prints out the distance, in meters, that light travels in one processor cycle. We use the hash mark (#) to introduce a comment. After the hash, we can write anything we want. The rest of the line is treated as a comment. The comment is not interpreted by the Python interpreter, but it is useful for humans reading the code.

Compute this by dividing the speed of light by the number of cycles per second.
```
speed_of_light = 299792458      # meters per second
cycles_per_second = 27000000000.  # 2.7 GHz
```
**Answer:** 
```
# Given the variables defined here, write Python 
# code that prints out the distance, in meters, 
# that light travels in one processor cycle. 

# speed_of_light in meters per second
# cycles_per_second is 2.7 GHz

speed_of_light = 299792458.0 
cycles_per_second = 2700000000.0
print speed_of_light / cycles_per_second
```
======
###Variables Can Vary
The value a variable refers to can change. When a variable name is used, it always refers to the last value assigned to that variable.

For example, you can change the value of **cycles_per_second**. Suppose you have a faster processor:

```
speed_of_light = 299792458# meters per second
cycles_per_second = 27000000000.# 2.7GHz
cycle_distance = speed_of_light / cycles_per_second
cycle_per_second = 2800000000.# 2.8 GHz
print cycle_distance
0.111034243704

cycle_distance = speed_of_light/ cycles_per_second
print cycle_distance
0.107068735
```
Since the value that a variable refers to can change, the same exact expression can have different values at the different times it is executed.

This gets more interesting when we use the same variable on both sides of an assignment. The right side is evaluated first, using the current value of the variable. Then the assignment is done using that value. In the following expressions, the value of days changes from 49 to 48 and then to 47 as the expression changes:
```
        days = 7 * 7# after the assignment, days refers to 49
        days = 48 # after the assignment, days refers to 48
        days = days - 1# after the assignment, days refers to 47
        days = days - 1# after the assignment, days refers to 46
```
It is important to remember that although we use = for assignment it does not mean equality. You should think of the = sign in Python as an arrow, ← , showing that the value the right side evaluates to is being assigned to the variable name on the left side.
======
###Quiz 8: Varying Variables Quiz 1
What is the value of hours after running this code:
```
        hours = 9
        hours = hours + 1
        hours = hours * 2
```
* a. 9
* b. 10
* c. 18
* d. 20
* e. 22
* f. Error

**Answer:** (d)

======

###Quiz 9: Varying Variables Quiz 2

What is the value of seconds after running this code:

```
minutes = minutes + 1
seconds = minutes * 60
```
**Answer:** Error

For Python to be able to output a result, you always need to define a variable by assigning a value to it, before using it.

```
minutes = 30
minutes = minutes +1
seconds = minutes * 60
print seconds
1860
```
