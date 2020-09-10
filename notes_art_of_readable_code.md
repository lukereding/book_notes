# The art of readable code

__Main idea__: Code should be written to minimize the time it takes for someone to understand it

## naming things

- Think of names is tiny comments. Be specific in concrete when you name things. Put more time and thought into naming variables that are more important are in scope for longer.

- When naming things, ask yourself what other interpretations could there be for a given name.

## consistency

- Use a format or to ensure code looks consistent.

- Use blocks of text to group related lines

## comments

- The goal of comments: you want your comments to enable the reader to know is much as the writer of the code knew when she was writing the code.

- Good code > bad code + good comments

- Use comments to provide context around why certain decisions were made or what the trade-offs were

- Try to anticipate questions or problems the reader might have as they read through your code. Use comments to head off those questions

- Don't comment what can be derived from the code or "crutch comments" and make up for bad code

## control flow

- Simplify our control flow logic to be as "natural" as possible

- The left-hand side of the expression should be the thing being interrogated. The right hand side should be the expression being compared against, whose value is more constant

- Pay attention to order; put positive simple cases first

- Return from functions as soon as possible, i.e., "return early" where it makes sense

- If you find yourself using lots of complex logic, step back and ask whether solving the "opposite" problem is easier

## variables 

- Shrink the scope of your variables wherever possible. People can only keep so many things in their heads at once, and by shrinking the scope of your variables, you make the reader's job easier

- Preferred immutable variables I said Constance are easier to reason about than variables that change constantly

## refactoring

- If your function is solving other problems besides the core problem, abstract that problem out into a new function, i.e., "look for unrelated sub-problems". It's easier to think about functions to do a single thing.

- If you find yourself copying and pasting a lot, that's a sign that you need to put that code into a function.

- If you're working with a library that has a crappy interface, you could always write your own wrapper functions to make the interface clear in your code more readable

- Common pattern: set a default value first and see if you can replace it with something more meaningful from the data of your person

## expressing yourself through code

- Your code should do one thing at a time. To help you do this, first list what your code is doing, then group similar tasks together or create separate functions

- Describe what the code needs to do, then write the code in a way that matches that description

- Don't write superfluous code. If you can, try solving a simpler problem or know where you can cut; knowing the standard library in the language that you're using can also be quite helpful

## testing

- Test code should be readable, too!

- Given/when/then can be helpful when writing tests

- Pick the simplest set of inputs that completely exercise your code

- Write different tests to test for different aspects of the functionality. Don't try to put it on a single test

- Name tests for what they're testing
