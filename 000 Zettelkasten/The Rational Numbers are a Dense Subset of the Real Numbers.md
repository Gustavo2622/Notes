202502261731

Status: #needs_more_references 

Tags: #theorem

# The [[Rational Numbers]] are [[Dense Subset]] of the Real Numbers

This means that, for every nonempty [[Open Set|open set]], there exists a number $q \in \mathbb{Q}$ that belongs to that set.

Since the [[Open Interval|open intervals]] form a [[Basis for a Topology|basis]] for the [[Standard Real Line Topology]], it suffices to show that each such interval contains a rational number.  
# Motivation
# Examples

- $\sqrt{2} < \frac{3}{2} < \sqrt{5}$ 
# Proof

Let $l < r \in \mathbb{R}$.

Using the [[Archimedean Property of the Rational Numbers in the Real Numbers]], there exists a number $m \in \mathbb{N}$ such that $\frac{1}{m} < r - l$. 

Using this property again, we can see that the set $\{n : n \in \mathbb{N} \wedge r*m < n\}$ is non-empty. Let $n + 1$ be the smallest element in this set (by [[Natural Numbers are a Well-Founded Set]]). Then we have that $l*m < n$ by $1 + l*m < r*m < r*m$. 

Therefore $l*m < n < r*m$ which implies that $l < \frac{n}{m} < r$.

# Corollaries

- Any real number can be arbitrarily well approximated by rationals: 
	- $\forall_{r \in \mathbb{R}}\forall_{\epsilon \in \mathbb{R}^+} \exists_{q \in \mathbb{Q}}\ q \in (r - \epsilon, r + \epsilon)$ 

# References

*Need to add*