---
layout: page
permalink: /csc348_notes/
---

**CSC 348 Notes**
----------------

Logic and Proofs
Propostional Logic
Proposition - Declarative sentence either true or false, but not both. States a fact. Letters (like "p" and "q" are used as propositional variables
The turth value of a proposition is true(T) if it is a true proposition and false(F) if it is a false proposition
Logic began with Aristote 2300 years ago

Let "p" be a proposition. The negation of p (~p) is the statement "It is not the case that p"

Conjunction of p and q (p /\ q) (logically equivalent of && in Java and C)
True when both p and q are true; false otherwise

Disjunction of p and q (p \/ q) (logically equivalent of || in Java and C)
True when either p or q is true; false otherwise

Exclusive Or (XOR) of p and q
XOR is true when only one of p and q is true; false otherwise

Conditional Statements: p -> q, "If p is true, then q is true"
p->q is false when p is true and q is false; otherwise true
p is considered the hypothesis and q is the conclusion

q->p is the converse of p->q
~q->~p is the contrapositive of p->q
~p->~q is the inverse of p->q

Contrapositives are logically equivalent to the conditional statement

Biconditional Statement: p <-> q "p if and only if q"
True if p and q have the same truth value; false otherwise

Order of Operations with logical operators
1. ~ Negation
2. /\ And (Conjunction)
3. \\/ Or (Disjunction)
4. -> Implication
5. <-> Biconditional

Parenthesis are used to clarify the intent with compound propositions

A bit is a symbol: 0 (False) or 1 (True)

Bit String: Length is the number of bits. After bitwise OR, AND, or XOR on the bit string, the resulting string will be the same length as the original. Inputs must be the same length.

Applications to Propositional Logic

A compound proposition that is always true no matter what the values of the propositional variables is called a tautology

A compound propositon that is always false is a contradiction

A compound proposition that is neither a tautology or contradiction is called a contingency

DeMorgan's Laws
1. ~(p /\ q) is logically equivalent to ~p \/ ~q
2.  ~(p \/ q) is logically equivalent to ~p /\ ~q

Distributive Law of Disjunction
p \/ (q /\ r) is logically equivalent to (p \/ q) /\ (p \/ r)

A compound proposition is satisfiable if there is an assignment of truth values to its variables that make it true. Otherwise it is called unsatisfiable

Predicate Logic
Example: x + 4 = 17
Variable "x" is the subject of the statement, " + 4 = 17" is the predicate

P(x) is the propositional function of predicate P at x
P(4) is a proposition and its truth value is false. ( 4 + 4 is not = to 17)

Let F(x,y,z) be the propositional function "x^2 + 2y = z"
What is F(1,1,1)? False
What is F(1,2,5)? True

The universal quantification of P(x) is the statement "P(x) for all values of x in the domain"

The existential quantification of P(x) is the statement " There exists an element in the doman, x, such that P(x) is true"

The uniqueness quantifier states that there exists an unique x in the domain such that P(x) is true

Introduction to Proofs
Proof - Valid arugment that establishes the truth of a mathematical statement

Theorem is a statement that can be shown to be true (usually via a proof)

A lemma is a small, easy to prove theorem. Plural: lemmata

A corallary is a theorem that can be established (almost) directly from a proven theorem.

A conjecture is a statement that is being proposed to be a true statement. "I wonder if this is true..."
Look for counter examples
Proof Techniques

Direct Proofs - Suppose p and try to prove q
Contrapositive Proofs - Suppose ~q and try to get to ~p
Contradiction Proofs - Suppose p and ~q, arrive at something absurd
Equivalence Proofs - Break up into two smaller lemmata, prove the lemmata
Exhaustive Proofs - Prove the elements in the domain, make sure to cover all cases
Without Loss of Generality - Fix the 










I'll upload the notes that I've taken in class here. This will probably be for my own personal reference.

[Return to Course Notes](https://jonscott20.github.io/course_notes/)
