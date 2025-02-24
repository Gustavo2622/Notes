202502131716

Status: #transient

Tags: #theorem

Top Links: [[Cryptography]]

# ROM is at least as strong as the Ideal Cipher Model

The [[Random Oracle]] model is at least as strong as the [[Ideal Cipher]] Model since there is an [[Indifferentiable Construction of Cryptographic Primitives |indifferentiable construction]] of a random oracle from an ideal cipher.

This construction is based on the [[Luby-Rackoff Construction]] and is exemplified in the following diagram:

![[Ideal Cipher from Random Oracle Indifferentiable Construction.jpg]]


## Proof

By prepending the k-bit key to the inputs to the inner RO functions ($F_i$ in the diagram above) it is possible to construct a family of 2ˆk random permutations, so it suffices to see how to construct a random permutation from the random oracle. --*expand this and see why it is true*--

## Relation to Luby-Rackoff Indistinguishability

The original [[Luby-Rackoff Construction]] is proven to be a [[Pseudo-Random Permutation]] given only 4 round of [[Pseudo-Random Function]] calls in the [[Cryptoraphic Primitive Indistinguishability|indistinguishability]] model. The intuition behind the difference in security is that in the [[Indifferentiable Construction of Cryptographic Primitives|indifferentiability]] model the adversary can query the inner [[Pseudo-Random Function|PRFs]] directly, while in the other case it cannot.


---
# References

- The Random Oracle Model and the Ideal Cipher Model are Equivalent; Coron, Patarin, Seurin