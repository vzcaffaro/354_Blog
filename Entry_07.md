# Entry 07

### Thoughts on Assignment 2

The hardest part of Assignment 2 for me initially was Part 1. 
While we have had some practice with Haskell, looking at the grammar and interpreter was quite a shock.
Specifically, changing the interpreter was a tall task for my existing skill set.
I could not understand the big picture of the interpreter, and how evalCBN and subst worked together.
After receiving some hand-holding, I was able to realize the interpreter is mostly just connecting our grammar to the existing syntax of Haskell.

Part 2 proved trivial, it mostly consisted of transferring the algorithms for multiplication and factorial, explored in Assingment 1 and in lecture, into our new programming language.

Part 3 was a fun prompt to follow.

Expanding upon the interpreter simply required pattern matching.
The head an tail functions were executed by recognizing the argument as a list then breaking it into its head and tail.
THe ENil function initially confused me.
Once I realized that evaluating an empty list hsould simply return the empty list, this issue was resolved.
Another issue we encountered was not changing our coercions in the grammar.
This resulted in incorrect inheritence of our expressions, which caused issues with parsing.

Writing the functions for less, makeLists, merge, and mergeLists took quite some time. The process was mostly that of 
trial-and-error, testing my ideas with inputs and comparing the outputted value with the expected output. Mergelists was 
definitely the most complex of these, and I finally resolved it by writing down the sequence of comparisons and replacements. 
This process allowed me to detach from the syntax and consider the concept of mergesort. Once I had done this, it was a simple 
task of making the syntax of our new programming language follow this concept.
Being able to see the heirarchy of functions in each testing file also helped visualize how functions work, behind the scenese.
