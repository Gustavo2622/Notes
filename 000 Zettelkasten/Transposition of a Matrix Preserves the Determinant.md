202503031650

Status: #needs_more_references  #missing_details

Tags: #theorem

# Transposition of a Matrix Preserves the Determinant

Let $M$ be a matrix (with entries in ???) and let $M^{T}$ be it's [[Transpose of a Matrix|transpose]].

Then the [[Determinant of a matrix|determinant]] of $M$ is that same as that of $M^T$ .

$$
	det(M) = det(M^T)
$$

# Motivation

It is natural to expect some relation between the determinant of a matrix and that of it's tranpose given the close relashionship between these two matrices.
This theorem shows that the relation we do get is the simplest possbie: equality.
# Examples

$$
det \left( \begin{bmatrix}
  1 & 2 & 3 \\
  4 & 5 & 6 \\
  7 & 8 & 9 
\end{bmatrix} \right)
=
det \left( \begin{bmatrix}
  1 & 4 & 7 \\
  2 & 5 & 8 \\
  3 & 6 & 9 
\end{bmatrix} \right)
$$

# Proof

## Proof using [[Matrix Row Reduction]]

Let $M$ be a matrix. We can perform row reduction on $M$ to obtain a decomposition:
$M = (E_0 E_1 E_2 \dots E_n) * N$, where $E_i$ are [[Elementary Matrices]] and $N$ is a [[Row-Echelon Form Matrix]].
Since [[Matrix Determinant is Multiplicative]] and [[Matrix Transpose is an Anti-Involution]], we can reduce the proof to the cases where $M$ is an [[Elementary Matrices|elementary matrix]] or a [[Row-Echelon Form Matrix]].
### [[Elementary Matrices]]

Here can can see directly that the transpose of an elementary matrix has the same determinant as itself by case analysis:
- Matrix to switch two adjacent rows: is self-transpose, therefore the stament is trivial in this case. 
$$
\begin{bmatrix}
	1      &        & \dots & \dots &        & 0      \\
	       & \ddots &       &       &        &        \\
	\vdots &        & 0     & 1     &        & \vdots \\
	\vdots &        & 1     & 0     &        & \vdots \\
	       &        &       &       & \ddots &        \\
	0      &        & \dots & \dots &        & 1
\end{bmatrix}
$$
- Matrix to add a multiple of a row to another: tranpose is still upper or lower triangular (upper if original is lower and vice-versa), so the determinant is still the product of the diagonal entries, which are preseved by transposition.
$$
\begin{bmatrix}
	1      &        & \dots & \dots &        & 0      \\
	       & \ddots &       &       &        &        \\
	\vdots &        & 1     & a     &        & \vdots \\
	\vdots &        & 0     & 1     &        & \vdots \\
	       &        &       &       & \ddots &        \\
	0      &        & \dots & \dots &        & 1
\end{bmatrix}
$$
- Matrix to multiply a row by a constant: self-tranpose, therefore the statement is trivial in this case.
$$
\begin{bmatrix}
	1      &        & \dots & \dots &        & 0      \\
	       & \ddots &       &       &        &        \\
	\vdots &        & 1     & 0     &        & \vdots \\
	\vdots &        & 0     & a     &        & \vdots \\
	       &        &       &       & \ddots &        \\
	0      &        & \dots & \dots &        & 1
\end{bmatrix}
$$

# Corollaries

- Determinant of [[Orthogonal Matrix]] is either 1 or -1. 
# References