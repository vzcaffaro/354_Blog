# Entry 06

### Thoughts on Lecture

Now that we can look at an ARS and its schema of rules, we must explore invariants as a method of both pattern matching and problem solving,
Officially, an invariant (represented as a function f) conforms to the following statement:
- iff a -> b, then f(a) = f(b)

In most reduction systems, we can look at the total number of each element.
These systems must be confluent and terminating.
If the ARS follows a specific form, we may be able to perform modulus operations on the total number, based on the rewrite rules for that letter.

An equivalence class is comprised of both an invariant and its unique normal form.
The use of equivalence classes can help to organize the reductions of an ARS, and to account for all possibilities.

While the concept of an invariant may seem confusing, in essence it is just a function that is used to compare "words" and whether they have the same normal form.
