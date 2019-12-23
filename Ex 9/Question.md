# Palindrome Checking

As Keg is primarily used for code golf competitions, it is a good idea to learn about using Keg for such purposes. Throughout this exercise, you will learn about:

- Comments
- Restricted source challenges
- Algorithmic thinking in Keg

## The Challenge

I want you to write a program that :

- Takes a series of characters as input
- If the string is a palindrome (reads the same backwards and forwards), print `1`
- Otherwise, print `0`

But here's the catch... Your program itself must be a palindrome.

## A Suggested Approach

- Although it may seem like the `^` command (reverse stack) could be helpful, I suggest that you stick to stack shifting to solve this problem.
- It is good to know that palindromes can be checked one pair of letters at a time. Consider the following :

    abccba

If the above string is left shifted once, it turns into `bccbaa`. This way, you can compare the first and last letter of the string easily. Repeat this while the length of the stack is bigger than 1 and you've got a working solution.

- Store the result of each comparison in the register by multiplying it each time (`=&*&`)

- Consequently, you'll need to initialise the register to `1` so that truthy comparisons don't get turned into falsely values via multiplication by 0

- To comply with the restricted source requirement, simply start a comment (using `#`) and place the source code in reverse.

- The input will _not_ contain any newlines

- `())(` is a palindrome. `()()` isn't. 
