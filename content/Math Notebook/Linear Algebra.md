


## Symmetric Matrix (Assume $\mathbb{R}^{n\times n}$)

> [!definition]
> A real symmetric matrix satisfies
> $$
> S = S^T
> $$

> [!property]
> - Has $n$ real eigenvalues $\lambda_1, \dots, \lambda_n$
> - Has $n$ orthonormal eigenvectors $q_1, \dots, q_n \in \mathbb{R}^n$ 
> - The \# of positive eigenvalues = \# of positive pivots. In fact, for symmetric real matrix, the signs of the eigenvalues are the same as those of the pivots

> [!theorem] Spectral Decomposition 
> $$
> S = Q \Lambda Q^{-1} = Q \Lambda Q^H = \sum_{i=1}^n \lambda_i q_i q_i^H
> $$
> The theorem applies to complex case as well

---

## Real Anti-Symmetric Matrix

> [!definition]
> A real matrix satisfying
> $$
> A = -A^T
> $$




> [!result]
> For any real vector $x$:
> $$
> x^T A x = 0
> $$
> $$
> \det(A) \ge 0
> $$
> for $3\times 3$ case, $I\pm A$ is invertible and $B=(I+A)(I-A)^{-1}$ are orthogonal



---

## Complex Eigenvalues (Real Matrices)

> [!property]
> If $Ax = \lambda x$, then
> $$
> A \bar{x} = \bar{\lambda} \bar{x}
> $$
> Eigenvalues come in conjugate pairs. The real and complex part of $x$ are not linearly dependent here.

---

## Orthogonal Matrices

> [!definition]
> $$
> Q^T Q = I
> $$

> [!property]
> Eigenvalues satisfy
> $$
> |\lambda| = 1
> $$

---

## Schur’s Theorem

> [!theorem]
> **Schur Decomposition**  
> Every square complex matrix can be written as
>
> $$
> A = Q T Q^{-1}
> $$
>
> where:
> - $Q^{-1} = Q^H$ (unitary)
> - $T$ is upper triangular
> - Eigenvalues appear on the diagonal of $T$
>
> If $A$ is real and the eigenvalues of $A$ are real, then $Q$ and $T$ can be chosen real, and
>
> $$
> Q^T Q = I
> $$

---

## Positive Definite Matrix

> [!definition]
> A symmetric matrix $S$ is positive definite if
> $$
> x^T S x > 0 \quad \forall x \neq 0
> $$

> [!equivalent]
> - $\lambda_i > 0$  
> - All pivots $> 0$  
> - All leading principal minors (upper left determinants) $> 0$  

---

## Positive Semidefinite

> [!definition]
> $$
> x^T S x \ge 0
> $$

---

## Factorization Test

> [!theorem]
> $$
> S = A^T A
> $$

> [!result]
> - Independent columns is equivalent to $S$ being positive definite  
> - Dependent columns is equivalent to $S$ being semidefinite  

---

## Geometry

> [!intuition]
> $$
> x^T S x = 1
> $$
> - Ellipse if $S$ is PD  


---

## Change of Variables

> [!result]
> Let $y = Q^T x$:
> $$
> x^T S x = y^T \Lambda y = \sum_{i=1}^n \lambda_i y_i^2
> $$

---

## Bounds

> [!result]
> $$
> x^T A x \le c\, x^T x
> \quad \text{where } c = \max \lambda_i
> $$

---

## Closure

> [!theorem]
> If $S, T$ are positive definite, then
> $$
> S + T \text{ is positive definite}
> $$