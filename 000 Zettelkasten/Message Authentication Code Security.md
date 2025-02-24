202502211847

Status: #transient

Tags: #definition

Top Links: [[Cryptography]]

# Message Authentication Code Security

*Vague, expand on this*
Without access to the secret key, no [[Cryptographic Security Game|adversary]] restricted to [[Cryptographically Feasible Computation|feasible computation]] can win the following [[Cryptographic Security Game|game]] with [[Cryptographically Negligible Function|non-negligible]] probability:
- The adversary has access to a [[Message Authentication Code|MAC]]-[[Cryptographic Oracle|oracle]] (with the secret key embedded) and can ask for the generation and/or verification of MACs for arbitrary messages.
- The adversary wins if he can generate a fresh message (not asked to the oracle before) and the corresponding correct MAC.

A stronger version of this also requires that the adversary be unable to generate a different valid MAC for a message that he *may* have sent to the oracle (for a probabilistic MAC scheme).
# Motivation

The main importance of this definition is that if this holds for a given protocol, then no adversary can (plausibly) forge signatures for bad messages.
# Examples

# Related Theorems

# References