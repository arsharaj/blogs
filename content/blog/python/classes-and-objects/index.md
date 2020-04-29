---
title: Classes and Objects in Python
date: "2020-04-29T00:00:00.000Z"
description: "Classes and Objects in Python"
category: "python"
---

Understanding classes and objects is very important for making good
modules in Python and easy to use packages. Since classes and 
objects are the building blocks of object oriented programming simply called
as OOPs. You know that Python is an object oriented programming language
beacuse everything in python in object. From the basic variables to the 
complex functions and different collection.

If you ever used the **type()** function then it also returns the types in the 
form of classes. By this you could just estimate that how much are the classes
and objects integrated in Python.

So, let's get started with this concept of classes and objects in Python.

In lame terms, **Classes** is simply a blueprint for making objects.
Take an example of a architect who makes the blueprint of the building or society.
Now whenever he wants to make a building he will simply use that blueprint 
and make the building according to that plan. 

Similiarly, in programming also we make different classes so that whenever
we want to make something then we do not have to make the plan for every object.
Implementing classes and object is very easy in python since it is one of the syntax 
friendly language in the whole world.

Let's say we are making a class of Person...

Why? So that whenever we want
to make persons with different characteristics then we can use that Person class blueprint.

### Defining a Class

```python
class Person:
    def __init__(self, name, age):
        self.name = name
        self.age = age
```

Now, here I have introduced and couple of things.

- First of all **class** keyword is reserved in Python.
- Classes by default comes with **__init__()** function. This function is particularly used to 
instantiate the variables and methods whenever a new object is created. If you are familiar
with **constructors** in other programming languages then this function is something like that.
And if you are not, then it is also used to instantiate variables and methods
- The key factor to keep in mind is the **self** keyword. The self keyword is simply the instance of th
current class (here, Person). The name of this instance is not fixed. You can
give it the name whatever you like. but developers use this self as a naming convention.
- Always keep in mind that the self keyword could only be the first parameter in the function call.

### Methods inside Class
```python
class Person:
    def __init__(self, name, age):
        self.name = name
        self.age = age
    
    def printName(self):
        print("My name is : " + self.name)
```

Look at that self parameter in the method. It is used inside the method to 
access the variables in the class.
- Use the self parameter in the function whenever you want to access the variables outside the function and in the class.

### Creating Objects and accessing them

```python
class Person:
    def __init__(self, name, age):
        self.name = name
        self.age = age
    
    def printName(self):
        print("My name is : " + self.name)
    
p1 = Person("Ram", 20)
print(p1.name)
print(p1.age)
p1.printName()
```

The output look like this :
```bash
Ram
20
My name is : Ram
```

Now similiarly you can make multiple objects from the same class and extend it as per need.
```python
class Person:
    def __init__(self, name, age):
        self.name = name
        self.age = age
    
    def printName(self):
        print("My name is : " + self.name)
    
p1 = Person("Ram", 20)
p2 = Person("Shyam", 13)
p3 = Person("Raju", 24)
```

Soon, I will also tell you about inheritance in Python. 

Till then keep coding !!!