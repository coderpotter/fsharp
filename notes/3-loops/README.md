# Types of loops
## for...to and for...downto loops
A for loop is a repetition control structure that allows you to efficiently write a loop that needs to execute a specific number of times.
The syntax of a for...to loop in F# programming language is −
```f#
for var = start-expr to end-expr do
   ... // loop body
```
The syntax of a for...downto loop in F# programming language is −
```f#
for var = start-expr downto end-expr do
   ... // loop body
```
- Example 1 - The following program prints out the numbers 1 - 20 −
```f#
let main() =
   for i = 1 to 20 do
      printfn "i: %i" i
main()
```
When you compile and execute the program, it yields the following output −
```
i: 1
i: 2
i: 3
i: 4
i: 5
i: 6
i: 7
i: 8
i: 9
i: 10
i: 11
i: 12
i: 13
i: 14
i: 15
i: 16
i: 17
i: 18
i: 19
i: 20
```

- Example 2 - The following program counts in reverse and prints out the numbers 20 - 1 −
```f#
let main() =
   for i = 20 downto 1 do
      printfn "i: %i" i
main()
```
When you compile and execute the program, it yields the following output −
```
i: 20
i: 19
i: 18
i: 17
i: 16
i: 15
i: 14
i: 13
i: 12
i: 11
i: 10
i: 9
i: 8
i: 7
i: 6
i: 5
i: 4
i: 3
i: 2
i: 1
```

## for...in loop
This looping construct is used to iterate over the matches of a pattern in an enumerable collection such as a range expression, sequence, list, array, or other construct that supports enumeration.
```f#
// Looping over a list.
let list1 = [ 10; 25; 34; 45; 78 ]
for i in list1 do
   printfn "%d" i

// Looping over a sequence.
let seq1 = seq { for i in 1 .. 10 -> (i, i*i) }
for (a, asqr) in seq1 do
   printfn "%d squared is %d" a asqr
```
When you compile and execute the program, it yields the following output −
```
10
25
34
45
78
1 squared is 1
2 squared is 4
3 squared is 9
4 squared is 16
5 squared is 25
6 squared is 36
7 squared is 49
8 squared is 64
9 squared is 81
10 squared is 100
```

## while...do loop
The while...do expression is used to perform iterative execution while a specified test condition is true.
Syntax -
```f#
while test-expression do
   body-expression
```
The test-expression is evaluated first; if it is true, the body-expression is executed and the test expression is evaluated again. The body-expression must have type unit, i.e., it should not return any value. If the test expression is false, the iteration ends.
Example -
```f#
let mutable a = 10
while (a < 20) do
   printfn "value of a: %d" a
   a <- a + 1
```
When you compile and execute the program, it yields the following output −
```
value of a: 10
value of a: 11
value of a: 12
value of a: 13
value of a: 14
value of a: 15
value of a: 16
value of a: 17
value of a: 18
value of a: 19
```