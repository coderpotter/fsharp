# Learning Functional Programming with F#
This repo is just notes on functional programming and F#. Basic programs helpful in learning F# might be added.

## Acknowledgement
Almost all of this content is taken from [tutorialspoint fsharp](https://www.tutorialspoint.com/fsharp/index.htm) and [tutorialspoint functional programming](https://www.tutorialspoint.com/functional_programming/index.htm)

## Some Need-to-Knows
- Functional programming languages are categorized into two groups −
  1. Pure Functional Languages − Support only the functional paradigms. For example − Haskell.
  2. Impure Functional Languages − Support the functional paradigms and imperative style programming. For example − LISP.

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

