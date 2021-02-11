---
title: Object Oriented Programming
tags: []
---

# Object Oriented Programming

## Four Pillars of OOP

### Abstraction
### Encapsulation
Binds together the data and functions that manipulate the data, and that keeps both safe from outside interference and misuse. ***(Private, Public and Protected Keywords)***

Encapsulation is a *technique for minimizing interdependencies among separately-written modules by defining strict external interfaces.  The external interface of a module serves as a contract between the module and its clients*.

If clients depend only on the external interface, the module can be reimplemented without affecting any clients, so long as the new implementation supports the same (or an upward compatible) external interface.

Encapsulation prevents external code from being concerned with the internal workings of an object. This **facilitates code refactoring**, for example allowing the author of the class to change how objects of that class represent their data internally without changing any external code (as long as "public" method calls work the same way). 

To maximize the advantages of encapsulation, one should minimize the exposure of implementation details in external interfaces

It also encourages programmers to put all the code that is concerned with a certain set of data in the same class, which **organizes it for easy comprehension by other programmers**
### Inheritance
Inheritance allows programmers to create classes that are built upon existing classes, to specify a new implementation while maintaining the same behaviors (realizing an interface), **to reuse code and to independently extend original software via public classes and interfaces**. The relationships of objects or classes through inheritance give rise to a directed graph.

Class based Programming Languages -> Inheritance
Prototype based Programming Languages -> Delegation

### Polymorphism
Any problem that can be solved with polymorphism can be solved without it. However, the polymorphic solution will always be more elegant, more compact, and easier to follow. any alternative solution will involve either maintaining numerous variables, passing them as function arguments, and duplicating large amounts of code; or creating, maintaining, passing, and using arrays of function pointers. Polymorphism really is simple in comparison.

#### Function Binding
Normally, when the compiler processes a function it generates the machine code that corresponds to the function body and arranges for the machine code to be stored at some location in memory. Wherever that function is called, the compiler must "bind" the call to that location in memory. That is, the compiler generates instructions to jump to that location in memory, execute the function's instructions, and then return to the calling point. Binding takes place when the system identifies the address corresponding to a given function call and generates the instructions needed to jump to that address. So, for the function calls

1. c->draw();
2. r->draw();
3. t->draw();

the compiler is able to bind statement 1 to the Circle draw function, statement 2 to Rectangle, and statement 3 to Triangle. Three terms, all synonyms, are used to name and describe this kind of binding:

* compile time binding
* static binding
* early binding

These terms are all synonyms that mean the same thing: the compiler is able to bind a function call to a specific set of machine instructions at the time that the program is compiled.

**Polymorphism represents a different kind of function binding. Polymorphism is nothing more than delaying the function binding until the program is running!** This kind of binding is also known by several different names:

* **Run-time binding**
* **Late binding**
* **Dynamic binding**
* **Dynamic dispatch (calling a function is sometimes called dispatching the function)**
