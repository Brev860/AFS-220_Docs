# Week 3 Lecture - AFS220

Learnign goals for weeks 3 & 4 => This week our class time will focus on reviewing Agile PM while filing in some high level gaps in python & Django — paving way for the second half of the course where we will take a deep dive into data structures and algorithms.

## Agenda

    1) Weeks 1 & 2 Overview
    2) Python Review
    3) Introduction to Django

### 1. Weeks 1 & 2 overview

- Intro to Agile Project Management
- Kanban vs. Scrum
- Introduction to Python

### 2. Introduction to Python

#### **Distribution**

[Anaconda](https://www.anaconda.com/) is a distribution of the Python and R programming languages for scientific computing (data science, machine learning applications, large-scale data processing, predictive analytics, etc.), that aims to simplify package management and deployment.

Anaconda is most likely to feature rich for our general purposes. Try [miniconda](https://docs.conda.io/en/latest/miniconda.html) instead!

    Distributions of programming stacks and technologies will become more common as you expand outside of the MERN stack. Apollo and graphQL is a good example of a distributed system.

One of the best ways I have found to learn and teach python is by the [python tutorial](https://docs.python.org/3/tutorial/index.html) directly from their documentation. Don't forget to bookmark the [glossary](https://docs.python.org/3/glossary.html#glossary).

#### OOP

The 4 pillars of Object-Oriented Programming are:

1. Encapsulation

2. Abstraction

3. Inheritance

4. Polymorphism

##### **Encapsulation**

Encapsulation is accomplished when each object maintains a private state, inside a class. Other objects can not access this state directly, instead, they can only invoke a list of public functions. The object manages its own state via these functions and no other class can alter it unless explicitly allowed. In order to communicate with the object, you will need to utilize the methods provided. One way I like to think of encapsulation is by using the example of people and their dogs. If we want to apply encapsulation, we do so by encapsulating all “dog” logic into a Dog class. The “state” of the dog is in the private variables playful, hungry and energy and each of these variables has their respective fields.

There is also a private method: bark(). The dog class can call this whenever it wants, and the other classes can not tell the dog when to bark. There are also public methods such as sleep(), play() and eat() that are available to other classes. Each of these functions modifies the internal state of the Dog class and may invoke bark(), when this happens the private state and public methods are bonded.

##### **Abstraction**

Abstraction is an extension of encapsulation. It is the process of selecting data from a larger pool to show only the relevant details to the object. Suppose you want to create a dating application and you are asked to collect all the information about your users. You might receive the following data from your user: Full name, address, phone number, favorite food, favorite movie, hobbies, tax information, social security number, credit score. This amount of data is great however not all of it is required to create a dating profile. You only need to select the information that is pertinent to your dating application from that pool. Data like Full name, favorite food, favorite movie, and hobbies make sense for a dating application. The process of fetching/removing/selecting the user information from a larger pool is referred to as Abstraction. One of the advantages of Abstraction is being able to apply the same information you used for the dating application to other applications with little or no modification.

##### **Inheritance**

Inheritance is the ability of one object to acquire some/all properties of another object. For example, a child inherits the traits of his/her parents. With inheritance, reusability is a major advantage. You can reuse the fields and methods of the existing class. In Java, there are various types of inheritances: single, multiple, multilevel, hierarchical, and hybrid. For example, Apple is a fruit so assume that we have a class Fruit and a subclass of it named Apple. Our Apple acquires the properties of the Fruit class. Other classifications could be grape, pear, and mango, etc. Fruit defines a class of foods that are mature ovaries of a plant, fleshy, contains a large seed within or numerous tiny seeds. Apple the sub-class acquires these properties from Fruit and has some unique properties, which are different from other sub-classes of Fruit such as red, round, depression at the top.

##### **Polymorphism**

Polymorphism gives us a way to use a class exactly like its parent so there is no confusion with mixing types. This being said, each child sub-class keeps its own functions/methods as they are. If we had a superclass called Mammal that has a method called mammalSound(). The sub-classes of Mammals could be Dogs, whales, elephants, and horses. Each of these would have their own iteration of a mammal sound (dog-barks, whale-clicks).

    Can you think of examples of each pillar already from your JS learnings? Creating a project where you can clearly show examples of each pillar will be a huge step in your interview prep. -or- using examples from your portolio projects!

#### Intro

Python is simple to use, but it is a real programming language, offering much more structure and support for large programs than shell scripts or batch files can offer. On the other hand, Python also offers much more error checking than C, and, being a very-high-level language, it has high-level data types built in, such as flexible arrays and dictionaries. Because of its more general data types Python is applicable to a much larger problem domain than Awk or even Perl, yet many things are at least as easy in Python as in those languages.

Python allows you to split your program into modules that can be reused in other Python programs. It comes with a large collection of standard modules that you can use as the basis of your programs — or as examples to start learning to program in Python. Some of these modules provide things like file I/O, system calls, sockets, and even interfaces to graphical user interface toolkits like Tk.

Python is an interpreted language, which can save you considerable time during program development because no compilation and linking is necessary. The interpreter can be used interactively, which makes it easy to experiment with features of the language, to write throw-away programs, or to test functions during bottom-up program development. It is also a handy desk calculator.

Python enables programs to be written compactly and readably. Programs written in Python are typically much shorter than equivalent C, C++, or Java programs, for several reasons:

- the high-level data types allow you to express complex operations in a single statement

- statement grouping is done by indentation instead of beginning and ending brackets

- no variable or argument declarations are necessary

Python is extensible: if you know how to program in C it is easy to add a new built-in function or module to the interpreter, either to perform critical operations at maximum speed, or to link Python programs to libraries that may only be available in binary form (such as a vendor-specific graphics library). Once you are really hooked, you can link the Python interpreter into an application written in C and use it as an extension or command language for that application.

    By the way, the language is named after the BBC show “Monty Python’s Flying Circus” and has nothing to do with reptiles. Making references to Monty Python skits in documentation is not only allowed, it is encouraged!

[python cheat sheet](https://www.pythoncheatsheet.org/)

### 2. Django

    "The Web framework for perfectionists with deadlines"

[Django](https://www.djangoproject.com/start/) is a high-level Python Web framework that encourages rapid development and clean, [pragmatic](https://www.freecodecamp.org/news/thought-on-the-pragmatic-programmer/) design. Built by experienced developers, it takes care of much of the hassle of Web development, so you can focus on writing your app without needing to reinvent the wheel. It’s free and open source.

- Ridiculously fast: Django was designed to help developers take applications from concept to completion as quickly as possible.

- Reassuringly secure: Django takes security seriously and helps developers avoid many common security mistakes.

- Exceedingly scalable: Some of the busiest sites on the Web leverage Django’s ability to quickly and flexibly scale.

- Fully loaded: Django includes dozens of extras you can use to handle common Web development tasks. Django takes care of user authentication, content administration, site maps, RSS feeds, and many more tasks — right out of the box.

- Incredibly versatile: Companies, organizations and governments have used Django to build all sorts of things — from content management systems to social networks to scientific computing platforms.

