# Summate Positive Integers

Dynamic arithmetic is a very important part of life. Throughout this exercise, you will learn about:

- `While` loops
- Nice input
- (Optional) How to structure a post-test while loop

## The Challenge

I want you to write a program that:

- Takes user input as a number while the input is greater than 0
- Summates all the inputs
- Prints the summation as an integer

You will need to know these things:

- A `while` loop is written in the form of `{condition|code}`, where `condition` is a Keg expression to evaluate each iteration to determine whether or not `code` will be executed. 
- The `¿` command takes the next line of input and tries to evaluate it as first a decimal (float), an integer, a list and finally a string. 
- If you happen to have any extra data items on your stack at the end of execution, you can use `_` to remove items. In other words, `_` discards the top of the stack. 

## Post-Test Loops

Some languages like Java and the C family have `do-while` loop constructs. These loops are called post-test loops, as the evaluate the condition at the end of each iteration. While Keg's `while` loops are pre-test loops, they can be made post-test like so:

    1{|<code><condition>}

Where one replaces `<code>` with the usual code and `<condition>` with the loop condition. 
