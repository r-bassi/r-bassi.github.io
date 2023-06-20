---
layout: post
title: "Object Oriented Design Principles"
date: 2021-03-24
categories:
  - blog
tags:
  - object oriented design
  - design patterns
  - design principles
  - blog
---

# Object Oriented Design Principles

> ## Table of Contents
> 
> - [What is Object Oriented Design?](#intro)
> - [How to Organize Code](#organize)
> - [S O L I D](#solid)
> - [Information Hiding](#info-hide)
> - [Summary](#summary)

### <a name="intro"> What is Object Oriented Design? </a>

If you google "Software Design Principles", there are a **lot** of them. They all come back to one idea: the localization of reasoning. The differences are that they arise in various problematic situations, and call for different design remedies. It all points to one  principle, which is that changes should be ideally localized to one place, and that each place should correspond to one kind of change. If the class is aligned with one change, it is aligned with one behaviour or responsibility within the system.

### <a name="organize"> How to Organize Code </a>

We start with a change we want to make within our code. If the change is too difficult to make, for some reason or another, the change reveals a problematic lack of abstraction, also known as a code smell. We then discover what makes our code problematic and refactor our code to arrive at more principled code.

Principled code doesn’t start out that way. We look realistically at what we are trying to enable programmers to do with our code, what kind of change they want to make, and then emerge principled code through refactoring.
![](https://rohitbassi.net/images/organizecode.JPG)
<sub>*[What is the Law Of Demeter?](https://en.wikipedia.org/wiki/Law_of_Demeter)*</sub>

### <a name="solid"> S O L I D </a>
###### What is SOLID?
- <ins>**S**</ins>ingle Responsibility Principle

- <ins>**O**</ins>pen/Closed Principle

- <ins>**L**</ins>iskov Substitution Principle

- <ins>**I**</ins>nterface Segregation Principle

- <ins>**D**</ins>ependency Inversion Principle

SOLID is a nice combination of principles to remember because they give a good coverage of likely problems that a programmer can encounter, and from there you can better understand other design principles.

###### Single Responsibility Principle
- Every class or function in a program should have a responsibility of only a single component of the overall program's functionality

###### Open/Closed Principle
- A class must be closed for internal change but must be open for extensions. Design a class so that extensions can be modular, and provide new functionality by using the power of the inheritance within the language you are using.

###### Liskov Substitution Principle
- Simply put, a subclass should not break the expectations set by its superclass. Penguins do not live up to all the things the normal definition of what a Bird can do, so if a Penguin were a subclass of a Bird, that would break the Liskov Substitution Principle.

###### Interface Segregation Principle
- A client should not be forced to depend on methods that it does not use. Any class implementation should not contain methods that do not fit its abstraction. If the ISP is violated, then the SRP has also been violated.

###### Dependency Inversion Principle
- High-level modules should not depend on low-level modules, both should depend on abstractions. Details should also depend on abstractions, if the details change they should not affect the abstraction. 

### <a name="info-hide"> Information Hiding </a>

Information hiding is one of the most important design principles, one that has been around for a very long time. The idea is that the programmer makes decisions to hides certain implementations from the rest of the program. The main task is to decide which features should be hidden.

You should only expose necessary functions, and use abstraction to hide complexity. For example, the caller to a function should not have to assume anything about how the interface is implemented. The effects of internal changes should be localized, and by separating the design decisions that are likely to change, you protect other parts of the program from many modifications if the design is changed.

### <a name="summary"> Summary </a>

- Classes should do one thing, often that one thing aligns with the role of the class
- Depend on abstractions instead of implementations.
- Make sure your interfaces are role specific, and do fulfill only one role.
- Refactor your designs so that you can localize changes within the code.


To gain more experience with object oriented design principles, I recommend practicing recognizing code smells within your own code and thinking about how changes to your designs could violate any of the above principles. Once you have a solid grasp of SOLID, you will find that other coding principles are also based around this idea of localized changes and abstraction.
