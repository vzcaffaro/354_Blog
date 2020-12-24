# Entry 08

### THoughts on Assignment 3

The jump from LambdaNat to LambdaFun is significant, as should be expected for the transition from a functional to imperitave programming langauge.

Part 1 involved translating our solution for Assingment 2 into our new syntax.
This allowed us to further contemplate our solution, as we essentially changing the way our program matches patterns to behave as desired.

Part 2 was much more difficult. A CList essentially works as a linked list.
This seemed like a lot, especially as we had not dealt with addresses and pointers prior to this.
Initially, all of our attempts were completely ineffective, as we were forgetting to use the ! operator to dereference the argument.
Following this, our solution came from exhaustive experimentation, and close studying of the grammar for LambdaFun.
Interestingly enough, we chose to complete insert first.
This proved to be the most complex function as far as reordering the list went.
After finally finishing insert, the rest of the functions seemed much easier to implement.
The hardest part of the assignment definitely was learning the new syntax of our language, and more importantly how assignment was done and varied from pointers to values.
Adding the tests to the file and watching the terminal spit out an array of passed tests was a very satisfying feeling.
