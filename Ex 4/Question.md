# Even and Odd Numbers

The ability to repeat chunks of code within a program is an important part of any programming language. Throughout this exercise, you will learn about:

- `For` loops
- The modulus operator (`%`)
- How to manage a loop counter

## The Challenge

I want you to write a program that:

- Starts at the number 0, and:
- For each number from 0 to 100 (inclusive):
-   If the number is even, print the letter `E`
-   Otherwise: print the number
- Each number/letter is to be seperateed by a space

You will need to know these things:

- A `for` loop is written in the form of `(numberOfLoops|code)`, where `numberOfLoops` is the amount of times to repeat the loop and `code` is the code to execute through each iteration
- When a `for` loop isn't given an explicit `numberOfLoops`, the length of the stack is used
- The `%` pops two numbers (`a` and `b`) from the stack and pushes the result of `b % a`
-    `82%` would result in `0` as `8 % 2` is 0
-    `92%` would result in `1` as `9 % 2` is 1
- Any even number when divided by two will always be evenly divided. In other words, any even number % 2 = 0
- The `for` loop doesn't automatically increment the loop counter, meaning that it needs to be manually incremented.
- `:` will help ensure that the loop counter always stays on the stack. Consequently, the loop counter needs to be pushed before the start of the loop
