# Entry 05

### Thoughts on Lecture

Previously we defined an ARS as a set of elements and a set of relations between elements.
We said that an ARS must be confluent and terminating to be functional.

A confluent ARS demonstrates reduction of a "word" to a unique normal form, which is independant of the order the rewrite rules are implemented.

**Termination** indicates that an ARS will at some point in finite time reach the end of its computation and thereby, will terminate.
In other words, a terminating ARS will never enter an infinitely chaining reduction.
This can be identified by the absence of reflexive rewrite rules.

For an example: Let (A,->) be an ARS spanning elements {a,b}, and let relation -> be defined as:
- ab -> ba
- ba -> ab
Obviously, this is not a complete rewrite system.
For now, consider it a base that would be expanded upon.
At first glance, these two rules seem very helpful.
It could be reasoned that the rules allow us to reorder the elements any way we see fit.
Maybe this could allow us to "force" patterns for pattern-recognition (e.g. if our word is "aaaabb" and a rewrite rule exists such that baba -> " ").
Despite our initial reaction, *the ARS would not be terminating*.
This is due to the fact that the existence of such circular rewriting rules would enter the reduction into an infinitely chaining reduction, i.e. an infinite loop.

In essence, an ARS that does not terminate is not fully-functional and in some cases will never reduce to a normal form.
