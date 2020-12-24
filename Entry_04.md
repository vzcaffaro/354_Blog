# Entry 04

### Thoughts on Lecture
 
This week we introduced rewriting systems, better known as Abstract Reduction Systems (ARS). 
An ARS is composed of both a set of elements and a set of relations that certain elements posess.
For a set of elements A and a set or relations ->, the ARS is written as ( A , -> ).

ARSs can be very powerful tools of comparing equalities of elements, no matter what form they take.
An ARS can be implemented as an algorithm, and can output the reduced form of any inputted "word".
This technique can be implemented in Haskell or any other programming language.
For now, we will focus on the concept of ARSs rather than the Haskell-specific syntax.
This way, we will be able to utilize ARSs in any functional programming language, provided the simple task of learning that language's syntax.

For an ARS to function as we desire, it must be confluent.

**Confluence** is the property where: if there exists two or more routes in which a word may reduce, these subreductions will eventually join.
Essentially, an ARS is confluent if the order in which its rewrite rules are applied do not matter; the rewrite rules do not overlap.
It is important that each word in the set of elements has a normal form which (a) is unique; the word may not be reduced to nay other form, and (b) may not be further reduced.

If an ARS is confluent and terminating, it can be implented as an algorithm. Termination is detailed in the next blog entry.
 
