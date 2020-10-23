# Entry 01

### Thoughts on Lecture
Being a Computer Science major, I have accumulated some experience in coding with imperative languages. Honestly, before taking this class, I was unaware of the distinction between functional and imperative programming languages.

After the first week of lectures in Programming Languages, I feel mostly comfortable with the idea of a functional programming language. This is likely attributed to my background in Math, specifically Discrete Mathematics.

After the second lecture, the connection between Programming Languages and Discrete Math is only more apparent. List syntax is identical, the inability to assign variables is shared, and the power of the language comes from recursion. All-in-all, Haskell seems to be an ideal implementation of the problem-solving techniques taught in Discrete Math.

### Thoughts on Homework
After learning basic syntax for list operations in Haskell, we were asked to define the following functions:</br>
- select_evens
- select_odds
- member
- append
- revert
- less_equal

Selecting evens and odds proved to be quite simple, using Haskell built-in filter function. Member, append, and revert were all slightly more complex yet still easy to implement with a good understanding of list syntax. To implement less_equal, which checks each index of the list and compares it with the same index of another list to return a boolean, I wanted to use a simple for-loop. However, as these are not supported in Haskell, I would need to define the function using recursion, and I do not yet fully understand how I would go about checking each index let alone checking that the lists are of equal size. 

While I do like the format of Haskell's function definitions (input/output type checking, followed by a base case to exit function, followed by recursive definitions) I feel like the type declaration at the top of each function could be more explicit as to which is an input and which is an output. Either way, it is still fully functional as-is.</br>