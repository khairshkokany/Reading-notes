## Inheritance
- Inheritance enables you to create new classes that r-use, exxtend and midify the behavior defined in other classes
- The class whose members are inherited is called the base class.
- The class that inherits those members is called the derived class
  - the derived class can only have one direct base class
- When abase class declares a method as virtual, a derived class can override the methos with its own implemintation
- If you declare a class as abstract you will prevent direct instatiation by using the new operator

## Abstract & Sealed Classes
- The abstract key keyword enables you to create classes and class members that are incompete and must be implemented in a derived class
- The sealed keyword enables you to prevent the inherintance of a class or certain class members that were previously marked virtual
- Classes can be declared as abstract by putting hte keyword abstract before the class definition
  - i.e: public abstract class A
- Abstract classes cannot be instantiated. Their purpose is to provide a comin definition of a base class that multiple derived classes can share.
- Abstract methods have no implentation, so the method definition is followed by a semicolon
- Sealed class cannot be used as a base class nor an abstract class.

## Polymorphism
- Polymorphism is referred to as the 3rd pillar of object- oriented programming, after encapsulation and inheritance.
- At run time, objects of a derived class may be treated as objects of a base class in places such as method parameters and collections or arrays
- Base classes may define and implement virtual methods, and derived classes can override them, which means they provide their own definition and implementation. At run-time, when client code calls the method, the CLR looks up the run-time type of the object, and invokes that override of the virtual method
- Virtual methods allow you to work with groupd of related objects in a uniform way
- To solve a problem using polymorphism do the following
  - Create a class hierarchy in which each specific shape class derives from a common base class
  - Use a virtual method to invoke the appropiate methos on any derived class thorugh single call to the bases class emthod
 
 ## Object Oriented Programming
 - C# is an object oriented programming language
 - The 4 basic principle of Object-Oriented Programming are:
  - **Abstraction** Modeling the relevant attributes and interactions of entities as classes to define an abstract representation of a system.
  - **Encapsulation** Hiding the internal state and functionality of an object and only allowing access through a public set of functions.
  - **Inheritance** Ability to create new abstractions based on existing abstractions.
  - **Polymorphism** Ability to implement inherited properties or methods in different ways across multiple abstractions.