# Counting Down

Here's a good oppourtunity to re-inforce knowledge from the last 6 exercises. Throughout this exercise, you will learn about:

- Combining `for` and `while` loops
- The register
- The decrement operator

## The Challenge

I want you to write a program that:

- While the user input isn't negative:
-    Asks for a single integer, and
-    Prints every integer from 1 to that integer in descending order, then
-    Prints a newline
- Numbers are to be seperated by spaces

An example session of use would look like so: _Note that user input is shown as `>>>`

<!-- Wrapped in three backticks due to GitHub being a silly-billy and not rendering properly when using tab-formatted code blocks -->
<!-- Enjoy the rest your day! :p -->

```
>>> 5
5 4 3 2 1
>>> 4
4 3 2 1
>>> 10
10 9 8 7 6 5 4 3 2 1
>>> -1
```

You will need to know these things:

- The register is a kind of variable where data can be temporarily stored. It is accessed using the `&` command.
- The register can only be in either `set` or `get` mode at any time.
- When the register is in `set` mode, the top of the stack is popped and stored in the register
- When the register is in `get` mode, whatever is in the register is pushed onto the stack, leaving the register empty.
- Calling `&` will toggle the register between `get` and `set` mode. The register starts in `set` mode.
- The `;` command decrements the top of the stack by 1. It is equivalent to `1-`
- You will need a for loop inside of a while loop
- The `:` command will come in handy here to preserve the value of the register after it has been emptied.

## The Register -- Some Examples
### Example 1

_Assume the stack is already set to_ `[45, 2, l, 10]`

    &_&
    & #Register: 10, Stack: [45, 2, l]
    _ #Register: 10, Stack: [45, 2]
    & #Register: Empty, Stack: [45, 2, 10]
    
From this example, it can be seen that the register is kind of a safe-haven for stack items

### Example 2
_Assume the input provided is 3_

    0&(¿|&:.1+&)
    0&  #Register: 0, Stack: []
    (¿|&: #Register: Empty, Stack: [0, 0], Loop iteration: 1
    . #Register: Empty, Stack: [0]
    1+  #Register: Empty, Stack: [1]
    &)  #Register: 1, Stack: []
    (¿|&: #Register: Empty, Stack: [1, 1], Loop iteration: 2
    . #Register: Empty, Stack: [1]
    1+  #Register: Empty, Stack: [2]
    &)  #Register: 2, Stack: []
    (¿|&: #Register: Empty, Stack: [2, 2], Loop iteration: 3
    . #Register: Empty, Stack: [2]
    1+  #Register: Empty, Stack: [3]
    &)  #Register: 3, Stack: []
    
 From this example, it can be seen that the register is quite commonly used with the `:` command.
   
   
   
   
   
   
   
