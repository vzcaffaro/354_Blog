# Entry 02

### Thoughts on Lecture
This week we learned to define natural number recursively in Haskell. Once again, this is very similar to concepts discussed in Discrete Mathematics. While we define our recursive numbers so that (S (S (S (S O)))) is a representation of the number 4, the Discrete Math form would look like ((((0 ->) ->) ->) ->), where "->" means "next". 

However, our representation of numbers is not very efficient from a testing point-of-view.  Our goal is to program a functional calculator, and it gets annoying typing in add (S (S (S O))) (S (S (S (S O)))) to test basic functionality. To address this, we define our own data type "data Exp Num Int". This allows us to expedite the testing process by typing just Times (Num 8) (Num 3) for example. 

### Thoughts on Homework

The homework this week was actually quite enjoyable as it required me to think back to the theories discussed in Discrete Math in order to implement the functions. Luckily, I was able to use the algorithms we defined in MATH250 for counting, addition, subtraction, and division. Division was the only one that took some time, but I was able to solve it once I thought back to the basic algorithm for division. For div (Num n) (Num m), the quotient is incremented every time m goes into n. So we recursively define division to be:
	div :: NN -> NN -> NN
	div n O = error "cannot divide by zero"
	div O m = O
	div n m = if (less n m) then add O (div (subtr n m) m)
        	else add (S O) (div (subtr n m) m)
The last exercise of the homework was also optional but was well worth implementing. If you redefine all of your functions to return an Exp instead of NN, the calculation is made using the recursive set NN that we defined, but both input and output of the functions use Num Int, which makes the calculator much more readable and testable from a programmers perspective.</br>