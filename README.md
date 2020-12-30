# Learning Functional Programming with F#
This repo is just notes on functional programming and F#. Basic programs helpful in learning F# might be added.

## Acknowledgement
Almost all of this content is taken from [tutorialspoint fsharp](https://www.tutorialspoint.com/fsharp/index.htm) and [tutorialspoint functional programming](https://www.tutorialspoint.com/functional_programming/index.htm)

## Some Need-to-Knows
- Functional programming languages are categorized into two groups −
  1. Pure Functional Languages − Support only the functional paradigms. For example − Haskell.
  2. Impure Functional Languages − Support the functional paradigms and imperative style programming. For example − LISP.
- Data types -
  1. Fundamental data types − Predefined data types which are used by the programmer directly to store only one value as per requirement, i.e., integer type, character type, or floating type.
  2. Derived data types − Derived using built-in data type which are designed by the programmer to store multiple values of same type as per their requirement.
  3. User-defined data types − These data types are derived using built-in data types which are wrapped into a single a data type to store multiple values of either same type or different type or both as per the requirement.
- Lambda Calculus - A framework developed by Alonzo Church in 1930s to study computations with functions.
    - Function creation - Church introduced the notation λx.E to denote a function in which ‘x’ is a formal argument and ‘E’ is the functional body. These functions can be of without names and single arguments.
    - Function application − Church used the notation E1.E2 to denote the application of function E1 to actual argument E2. And all the functions are on single argument.
  - Syntax of Lambda Calculus: Lamdba calculus includes three different types of expressions, i.e.,
    - E :: = x(variables)
    - | E1 E2(function application)
    - | λx.E(function creation)
    Where λx.E is called Lambda abstraction and E is known as λ-expressions.

## Introduction to Functional Programming (FP)
- Characteristics of FP −
  - Designed on the concept of mathematical functions that use conditional expressions and recursion to perform computation.
  - Supports higher-order functions and lazy evaluation features.
  - *Don’t* support flow controls like loop statements and conditional statements like if-else and switch statements. They directly use the functions and functional calls.
  - Like OOP, FP languages support popular concepts such as Abstraction, Encapsulation, Inheritance, and Polymorphism.

- Advantages of FP -
  - Bugs-Free Code − FP does not support state, so there are no side-effect results and we can write error-free codes.
  - Efficient Parallel Programming − FP languages have **no** mutable state, so there are no state-change issues. One can program "Functions" to work parallel as "instructions". Such codes support easy reusability and testability.
  - Efficiency − Functional programs consist of independent units that can run concurrently. As a result, such programs are more efficient.
  - Supports Nested Functions
  - Lazy Evaluation − FP supports Lazy functional constructs like lazy lists, lazy maps, etc.

- Disadvantage (this repo is about FP so obviously there's only one :smirk:) of FP -
  - Requires a large memory space. As it does not have state, you need to create new objects every time to perform actions.
  
Functional Programming | Object-Oriented Programming
---|---
Uses Immutable data. | Uses Mutable data.
Follows Declarative Programming Model | Follows Imperative Programming Model
Focus is on **“What you are doing”** | Focus is on **“How you are doing”**
Supports parallel programming | Not suitable for parallel programming
Functions have no-side effects | Methods can produce serious side effects
Flow Control is done using function calls & function calls with recursion | Flow control is done using loops and conditional statements
Uses "Recursion" to iterate over collection data	| Uses "Loops" to iterate over collection data
Execution order of statements is not so important |	Execution order of statements is very important
Supports both "Abstraction over Data" and "Abstraction over Behavior" |	Supports only "Abstraction over Data"

## About F#
- Basic syntax of F# can be found in [this file](notes/intro.fsx) (taken from [F# for fun and profit](https://fsharpforfunandprofit.com/posts/fsharp-in-60-seconds//)).
- In F#, functions work like data types. You can declare and use a function in the same way like any other variable.
- In general, an F# application does not have any specific entry point. The compiler executes all top-level statements in the file from top to bottom. However, to follow procedural programming style, many applications keep a single top level statement that calls the main loop.
- An F# code file might begin with a number of open statements that is used to import namespaces.
- [keywords and data types](notes/1-syntax/README.md)
- [variables](notes/2-variables/README.md)
- [loops](notes/3-loops/README.md)
- [functions](notes/4-functions/README.md)
- [strings](notes/5-strings/README.md)
- [options](notes/6-options/README.md)