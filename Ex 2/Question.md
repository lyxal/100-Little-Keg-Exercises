# Comparison of Two Letters

What good is a programming/golfing language if you cannot tell if two objects are different? Throughout this exercise, you will learn about:

- `If` statements
- Comparison operators
- Using TIO for exercises

## The challenge

I want you to write a program that:

- Takes two letters as input (each on a new line)
- Checks if they are the same letter, and:
-  If they are: display the word `Same`
-  Otherwise: display the word `Different`

You will need to know these things:

- An `if` statement is written in the form of `[onTrue|onFalse]`, where `onTrue` is the code to execute if the top of the stack is non-zero and `onFalse` is an optional block of code to execute if the top of the stack is zero
- `If` statements pop the top of the stack, meaning it cannot be used later
- The `=` operator pops two values off the stack and pushes `1` if they are the same or `0` if they aren't
- Anything that is left on the stack at the end of execution is automatically printed if a print function hasn't already been called

## How to Use [Try It Online](https://tio.run/#)

When completing these exercises, it can be helpful to have an online testing playground. Such a useful playground is the Keg interpreter found [here](https://tio.run/#keg), which is kindly hosted by [DennisMitchell](https://github.com/DennisMitchell).
On Try It Online (TIO), there are three main fields which you will be interested in using:

- The `code` section
- The `input` section
- The `output` section

Your Keg program goes in the `code` section, any input goes in the `input` section and the output of your program will be shown in the `output` section.
Here is a test case for your program, which has an example input already provided. [Try it online!](https://tio.run/##y05N/w8EGVwZAA "Keg – Try It Online")
