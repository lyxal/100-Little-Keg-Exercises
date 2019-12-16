# Tell the time

Do you know that Keg can tell the time by writing just a one-liner? Throughout this exercise, you will learn about:

- Auto-completion of `If` statements
- A review of comparison/arithmetic operators
- Basic stack manipulation

## The challenge

I want you to write a program that:

- Takes a single letter as input
- Subtracts 64 from the ascii code of the letter, and
  - If the the value < 12 (i.e. character before `L`):
    -  Say `Good Morning!`
  -  Otherwise, if the ascii code = 12 (i.e. character is `L`):
    -  Say `Hello!`
  -  Otherwise:
    -  Say `Good Evening!`

You will need to know these things:

- `:` duplicates the last item of the stack, so `(I)` will become `(I,I)` (I stands for items in the stack, the top of the stack faces the right)
- `_` discards the last item of the stack, so `(I)` will become `()`
- `\` escapes the next character and push it onto the stack. Although pushing an alphanumeric character is possible with this instruction, it is good practice to only use it to escape Keg instructions.

Side note:

- You can drop the trailing `]`'s if they are on the end of the program. So `[iftrue|iffalse]` can become `[iftrue|iffalse` on the end of the program.
