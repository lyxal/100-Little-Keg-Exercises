# Basic Calculator

Congratulations! You are now 1/10th of the way through the 100 little Keg exercises! To celebrate, let's try a more complex and practical project. Throughout this exercise, you will learn about:

- Completing a project
- Switch-like statements

## Project Description

Y'know that nice expensive computer you have? We're gonna turn in into a machine that performs just like a $5.00 calculator would.

This program will take two real numbers, as well as an operator and perform the given calculation.

E.g.

	8
	27
	+

Will output `35` because `8 + 27 = 35`.

	10
	7
	-

Will output `3` as `10 - 7 = 3`

Consequently, it can be inferred that there will be three newline-seperated inputs: the first number, the second number and the operator (which will be in '+-*/') 

In order to determine which operator to apply, a switch statement is needed.

Here's some psuedocode:

	switch (op)
		case '+'
			add numbers
		case '-'
			subtract numbers
		case '*'
			multiply numbers
		case '/'
			divide numbers


A switch statement Keggified may look like so:

	:case=[codeOnMatch|:case2=|[codeOnMatch2...]]

