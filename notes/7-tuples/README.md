# Tuples
A tuple is a comma-separated collection of values. These are used for creating ad hoc data structures, which group together related values.

For example, `("Animesh Nighojkar", "Tampa", 7)` is a 3-tuple with two string values and an int value, it has the type `(string * string * int)`.

Tuples could be pairs, triples, and so on, of the same or different types.

Some examples −
```
// Tuple of two integers.
( 4, 5 )

// Triple of strings.
( "one", "two", "three" )

// Tuple of unknown types.
( a, b )

// Tuple that has mixed types.
( "Absolute Classes", 1, 2.0 )

// Tuple of integer expressions.
( a * 4, b + 7)
```

### Example
This program has a function that takes a tuple of four float values and returns the average −
```f#
let averageFour (a, b, c, d) =
   let sum = a + b + c + d
   sum / 4.0

let avg:float = averageFour (4.0, 5.1, 8.0, 12.0)
printfn "Avg of four numbers: %f" avg
```
When you compile and execute the program, it yields the following output −
```
Avg of four numbers: 7.275000
```

## Accessing Individual Tuple Members
The individual members of a tuple could be assessed and printed using pattern matching.

### Example
```f#
let display tuple1 =
   match tuple1 with
   | (a, b, c) -> printfn "Detailed Info: %A %A %A" a b c

display ("Animesh Nighojkar", "Tampa", 7)
```
When you compile and execute the program, it yields the following output −
```
Detailed Info: "Animesh Nighojkar", "Tampa", 7
```
F# has two built-in functions, `fst` and `snd`, which return the first and second items in a 2-tuple.

### Example
```f#
printfn "First member: %A" (fst(23, 30))
printfn "Second member: %A" (snd(23, 30))

printfn "First member: %A" (fst("Hello", "World!"))
printfn "Second member: %A" (snd("Hello", "World!"))

let nameTuple = ("Zara", "Ali")

printfn "First Name: %A" (fst nameTuple)
printfn "Second Name: %A" (snd nameTuple)
```
When you compile and execute the program, it yields the following output −
```
First member: 23
Second member: 30
First member: "Hello"
Second member: "World!"
First Name: "Zara"
Second Name: "Ali"
```