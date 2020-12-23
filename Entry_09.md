# Entry 09


### Thoughts on the Final

Question 3 on the final was very intriguing to me.
I've always found the roman numeral system to be interesting, so formulating rewrite rules captivated my attention.

Question 3.3 definitely stumped me for a minute. I was overthinking the process of adding two numbers, and the $ signs were throwing me off.
Part of me though the answer was $x$y$ -> xy, but the other part of me knew this was too simple and there had to be an algortithm to apply.
Sure enough, my answer came to me when I considered the algorithm for addition. All I had to do was pull one letter out at a time, and write out the cases for each letter.

I was also stuck on Question 3.4 for some time, but once I got past my issue with the $ signs and solved 3.3, I simply implemented the algorithm for multiplication from Assignment 1.
This was easy as we were dealing with basically the same data type. To expand this system to accomodate 3.5, I initially took a much more difficult and less reasonable approach.
I attempted to write a case for any numeral being multiplied, but I quickly found out this would not be an effective approach.
Instead, I figured it best to ungroup numerals (i.e. V -> IIIII) while keeping them inside the $ signs.
This allowed my initial algorithm of multiplication to keep working, while ensuring confluence as the ungrouping rules remained within the $ signs.

Of all the questions, the measure functions in 3.7 proved to be the most time consuming.
I was tired of using base-10 measure functions, yet I could not conceive a different measure function for 3.1/3.2.
A lazy comprimise to this was the octal number base.
While unfamiliar with octal, I learned hexadecimal earlier this year and, of course, have been familiar with base-10 all of my life.
Octal was very easy to learn, following the same form as base-10 and hex, just using 8 instead of 10 and 16.
It made sense to me that octal has been used in computers for quite some time, as each octal bit is simply 3 binary bits grouped.
One interesting thing I learned is that octal has been around for much longer than computers, as some civilizations use the spaces in>

For the remaining measure functions, I attempted to write them in the form of mathematical equations even though we had not really done that all year.
While it took many attempts, I felt my finals results accomplished the goal of the measure function.
For each measure function, my equation included incrementing the x and y values by one, then performing addition for 3.3 and multiplication for 3.4.
This results in each step of the reduction being one less than the previous. This was just what I needed, though I am not entirely sure it is correct.
As for the 3.6 functions, AddtoOrd was trivial as every case reduced the number of numerals, so I implemented another octal based measure function.
OrdtoAdd increased the number of numerals in each rewrite rule. For this, I could not use a base-10 system unless it was the base-10 system to the right of a decimal point (i.e. 10^-1, 10^-2, etc)
Instead, I implemented addition. This worked in this case because, for example, the numeral that represents 4 is IV, where the I is subractive. For our function, this evaluated to 6, which was greater than the 4 that the IIII evaluated to.

This was definitely an interesting problem, and I spent a lot of ti e thinking on it. 
My thoughts did not stop at the resolution of the problem, however, which I elaborate on in [Blog 10](https://github.com/vzcaffaro/354_Blog/blob/master/Entry_10.md)<br>


