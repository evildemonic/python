
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
