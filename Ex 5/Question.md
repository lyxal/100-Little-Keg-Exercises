# Print a 10x10 Grid of Asterisks

Asterisks are fun little symbols that can be used for numerous things! Throughout this exercise, you will learn about:

- Nested loops
- Different uses of newlines
- (Optional) The `-in` flag

## The Challenge

I want you to write a program that:

- Outputs the following text:

<pre>
**********
**********
**********
**********
**********
**********
**********
**********
**********
**********
</pre>

- (Note that trailing newlines are acceptable)
- The program **must not** hardcode the grid... it must use loops

You will need to know these things:

- Loops can be nested inside of each other like so: `(count1|(count2|code))`
- Newlines will automatically be pushed, and have an ascii value of `10`

## Extra Challenge
Newlines can sometimes be quite combersome within longer programs if they are used for decorative whitespace. That's why the `-in` (`--ignorenewlines`) flag was added to Keg. When present, it will treat newlines as if they weren't there, meaning they need to be escaped.
Try writing a solution to this problem using the `-in` flag. To add a flag on TIO, click on the arguments section, click `+ add` and type in the flag you want to use.
If you are using the offline Keg interpreter, execute it like so:

  python3 Keg.py <file> -in
