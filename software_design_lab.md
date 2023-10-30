# Software Design

### 1. What do we mean by coupling and cohesion when discussing structured design?

```
Coupling describes the relationships between classes. Coupling can be strong such as in inheritence where the classes are closely linked to one another or more loosely such as in an interface. 
Cohesion describes the relationships within a class. A cohesive class will incorporate different attributes together to serve a single purpose, wheras a lack of cohesion can lead to a class having more than a single purpose; violating the SOLID principles.
```

### 2. What is the difference between top-down and bottom-up design? Which best describes a function oriented design?

```
The top-down approach begins with the big picture of what the end result will look like, and then breaks it down into smaller managable parts. Each of those parts can be broken down again into smaller parts until the tasks become managable. These multiple parts can then be delegated to multiple people within a team.

The bottom-up approach is the reverse, starting with the smallest components and slowly building them up into a larger structure. It is more commonly used in OOP languages like Java. Bottom-up makes it easy to test small parts and build them up together, but the system as a whole cannot be tested until all of the parts beneath it have been assembled.
```

### 3. In which design methodology would a class diagram be most useful?

```
A class diagram would be most useful in a top-down methodology, because they fit in well with the idea of breaking the problem down into smaller pieces. If we start at a large problem, it can be broken down into classes and again into sub-classes which best fits top-down working.
```

### 4. What are the four pillars of object oriented programming? Give a single-sentence description of each.


```
- Abstraction is to take away some of the complexity of tasks by breaking them into clear, easy to understand parts
- Encapsulation occurs when an objects methods and variables are concealed within a class, hiding them from being accessed from outside their classes.
- Inheritance is when a child class inherits the properties of a parent class in order to reduce repeating the same code. It is an example of strong coupling.
- Polymorphism is when an object can be many different object types simultaniously, allowing it to use properties that belong to these different object types.
```

### 5. What is the strategy pattern? How would its implementation differ between a functional and object oriented system?

```
The stratergy pattern is a design pattern that allows the behaviour of an object to be dynamically allocated during runtime. In OOP, the delegator uses an abstract interface to interact with multiple different implementations of other interfaces and dynamically allocates the correct code for the given task. In functional programming, interfaces are not used; instead, higher-order functions are used to call other functions to delegate that way.
```

### 6. Imagine your is creating a new online payment system. In order to gain maximum market share it can't be tied to a particular sector - it needs to work just as well when ordering a takeaway as when buying a new coat. Which design methodology would you suggest following? Give some justification for your decision.

```
The stratergy pattern should be employed to allow different payments to be used interchangably at runtime. A bottom-up methodology would be used to make the system because it is simple to implement testing of small-scale modules. 
```