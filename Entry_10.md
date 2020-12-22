# Entry 10

### Thoughts on the Final

Question 3 on the final was very intriguing to me. 
I've always found the roman numeral system to be interesting, so formulating rewrite rules captivated my attention.

Of all the questions, the measure functions in 3.7 proved to be the most time consuming.
I was tired of using base-10 measure functions, yet I could not conceive a different measure function for 3.1/3.2.
A lazy comprimise to this was the octal number base.
While unfamiliar with octal, I learned hexadecimal earlier this year and, of course, have been familiar with base-10 all of my life.
Octal was very easy to learn, following the same form as base-10 and hex, just using 8 instead of 10 and 16.
It made sense to me that octal has been used in computers for quite some time, as each octal bit is simply 3 binary bits grouped.
One interesting thing I learned is that octal has been around for much longer than computers, as some civilizations use the spaces in-between their fingers to count rather than the actual fingers themselves.


### Thoughts Beyond the Final
While contemplating this problem, I couldn't help but think of writing a program to translate decimal numbers to numerals.
My first thought on implementing this was to simply turn the decimal x into x Is, but then I realized this would be highly inefficient for large numbers.
My solution to this would be to translate the number using its indeces seeing as they represent powers of 10.
Assuming the rightmost decimal to be index 0, the computation would be as follows:
- # Is = indx_0 % 5
- # Vs = indx_0 / 5
- # Xs = indx_1 % 5
- # Ls = indx_1 / 5
- # Cs = indx_2 % 5
- # Ds = indx_2 / 5
- # Ms = indx_3 + 10*indx_4 + 100*indx_5 and so on

While this in and of itself does not have many applications, I thought it would be interesting if one could come up with an encryption pattern using our ARSs.
While I am not familiar with existing encryption algorithms, I figured it would be possible if we wrote an ARS that takes in an ordinary Roman numeral and outputs a rewritten numeral with a different value. The decryption would be the reflexive opposite of this ARS.
For an example, the encryption ARS could rewrite V -> LII, or DC -> XC, while the decryption ARS would be flipped.
It is important that the ARS would both be confluent and terminating, as a nonconfluent system might corrupt data in the encryption-decryption process, and a non-terminating ARS would result in the program infinitely looping.
Data could be encrypted with the following sequence of events:

1. Convert binary to base-10 decimal
2. Convert base-10 decimal to roman numerals
3. Encrypt roman numeral using rewrite rules
4. Convert roman numeral to base-10 decimal
5. Convert base-10 decimal to binary

Then, the binary value could be transmitted knowing that if it is intercepted, the data would be nonsense until decrypted.
While I am sure the efficiency of this would be far inferior to existing encryption algorithms, it is just a thought, and one that would be fun to implement.
