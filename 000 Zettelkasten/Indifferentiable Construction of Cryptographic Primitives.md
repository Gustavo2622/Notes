202502131739

Status: #definition

Tags: [[Cryptography]]

# Indifferentiable Construction of Cryptographic Primitives

A [[Turing Machine]] C with oracle access to an [[Ideal Primitive]] F is said to be $(t_{D}, t_{S}, q, \epsilon)$-indifferentiable from an [[Ideal Primitive]] P if there exists a [[Computational Simulator|simulator]] S with oracle access to P and running in time at most $t_S$ such that for any [[Computational Distinguisher|distinguisher]] D running in time at most $t_D$ and making at most $q$ queries it holds that: $$ \left|Pr\left[D^{C^F, F} = 1\right] - Pr\left[D^{P^S, P} = 1\right]\right| < \epsilon $$ $C^F$ is simply said to be indifferentiable from P if $\epsilon$ is a [[Cryptographically Negligible Function|negligible function]] of the [[Security Parameter]] n, for polynomially bounded $q, t_D, t_S$.
# Motivation

This comes as an extension of [[Cryptoraphic Primitive Indistinguishability]] in cases where the two scenarios have different conditions (e.g. a different interface, different inner functions to call) but we still want to show that given one primitive we can construct the other in a way which loses no security.
# Examples

- A [[Random Oracle]] can be indifferentiably constructed from an [[Ideal Cipher]]
- An [[Ideal Cipher]] can be indifferentiably constructed from a [[Random Oracle]]
# Related Theorems

# References

- The Random Oracle Model and the Ideal Cipher Model are Equivalent; Coron, Patarin, Seurin