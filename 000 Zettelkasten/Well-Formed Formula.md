202502251258

Status: #needs_more_references

Tags: #definition
# Well-Formed Formula

A *Well-Formed Formula* (or *wff*) is a syntactically valid statement in some [[Logical Language]].

They are generally defined out of a few base cases of valid *wff*s along with composition rules for getting new valid *wff*s out of other ones. ([[Composability multiplies effectiveness]])
# Motivation

This definition comes from the attempt to distuinguish syntax and semantics in logic. That is, to distinguish the language in which logical propositions are expressed from the actual meaning of said propositions (in a given [[Logical Interpretation]]).
# Examples

## [[Propositional Logic]]

In propositional logic, *wff*s are built up of symbols (representing logical variables) and [[Logical Connective|logical connetives]].

An example of such a *wff* is: $P \Rightarrow Q$.

## [[First Order Logic]]

In first order logic, the *wff*s are:
- Propositional Logic *wff*s
- $\forall_x W(x)$, where $W(x)$ is a *wff* and $x$ is a [[Free Variable]] in $W$.
- $\exists_x W(x)$, where $W(x)$ is a *wff* and $x$ is a [[Free Variable]] in $W$.

An example of such a *wff* is the [[Integer Induction]] principle (for a single predicate P):
$$ 
P(0)\ \wedge\ (\ \forall_n\ P(n) \Rightarrow P(S(n))\ ) \Rightarrow \forall_n\ P(n)
$$

# Related Theorems

# References

- [[Beginning Mathematical Logic: A Study Guide; Peter Smith]]