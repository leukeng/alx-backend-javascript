SOLUTION TO ES6 CLASSES

Classes are a template for creating objects. They encapsulate data with code to work on that data. Classes in JS are built on prototypes but also have some syntax and semantics that are unique to classes.

For more examples and explanations, see the Using classes guide.

Description
Defining classes
Classes are in fact "special functions", and just as you can define function expressions and function declarations, a class can be defined in two ways: a class expression or a class declaration.

Class body
The body of a class is the part that is in curly braces {}. This is where you define class members, such as methods or constructor.

The body of a class is executed in strict mode even without the "use strict" directive.

A class element can be characterized by three aspects:

Kind: Getter, setter, method, or field
Location: Static or instance
Visibility: Public or private
Together, they add up to 16 possible combinations. To divide the reference more logically and avoid overlapping content, the different elements are introduced in detail in different pages:
