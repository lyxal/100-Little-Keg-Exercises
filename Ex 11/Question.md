# Average Function

Functions are amazing features within any programming language that allow long chunks of code to be grouped together and be given a name. Throughout this exercise, you will learn about:

- Functions
   - Defining them
   - Calling them

## The Challenge

I want you to write a _function_ called `f` that:

- Takes 5 numeric parameters, and
- Returns the average of the numbers

## Functions in Keg

Obviously, in order to complete this exercise, you will need to know about how to write a function. 

Let's take a look at a simple example function as it would be written in python:

    def sub_three(num):
        return num - 3

Or in Java

    public int sub_three(int num) {
        return num - 3;
    } 

As you can see, this function takes a single number and decrements that number by 3.

In Keg, `sub_three` would look like this:

    @subThree 1|3-ƒ

While this may look confusing at first, the function structure is actually quite logical:

- The `@` symbol starts a function definition
- Then the function name is given (in this case, it is `subThree`). Note that function names can only contain uppercase and lowercase letters
- Then the number of parameters is given. This represents the number of items popped from the main stack to put onto the function's stack (think of this as a local scope)
- The `|` then designates that the function definition follows
- Finally, the `ƒ` closes the function

If we wanted to call our `subThree` function, we would do it like this:

    @subThreeƒ

Now don't be confused: the `@` still defines a function, but only if there is a `|` to specify the function definition. Othwrwise, it will try to call the function.
