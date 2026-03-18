I added this shit, give me money$


## Symmetric Matrix (Real)

> [!definition]
> A real symmetric matrix satisfies
> $$
> S = S^T
> $$

> [!property]
> - Has $n$ real eigenvalues $\lambda_1, \dots, \lambda_n$
> - Has $n$ orthonormal eigenvectors $q_1, \dots, q_n$

^8b3e0a

> [!theorem] Spectral Decomposition
> $$
> S = Q \Lambda Q^{-1} = Q \Lambda Q^T = \sum_{i=1}^n \lambda_i q_i q_i^T
> $$

---

## Anti-Symmetric Matrix

> [!definition]
> A matrix satisfies
> $$
> A = -A^T
> $$

> [!property]
> - Eigenvalues are purely imaginary  
> - Eigenvectors can be chosen orthonormal (complex)

> [!result]
> For any real vector $x$:
> $$
> x^T A x = 0
> $$

> [!result]
> $$
> \det(A) \ge 0
> $$

---

## Complex Eigenvalues (Real Matrices)

> [!property]
> If $Ax = \lambda x$, then
> $$
> A \bar{x} = \bar{\lambda} \bar{x}
> $$
> Eigenvalues come in conjugate pairs.

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
> Every square matrix can be written as
> $$
> A = Q T Q^{-1}
> $$

> [!property]
> - $Q^{-1} = Q^H$ (unitary)  
> - $T$ is upper triangular  
> - Eigenvalues appear on the diagonal  

> [!note]
> If eigenvalues are real, $Q$ can be chosen real:
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
> - All leading principal minors $> 0$  

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
> - Independent columns → positive definite  
> - Dependent columns → semidefinite  

---

## Geometry

> [!intuition]
> $$
> x^T S x = 1
> $$
> - Ellipse if $S$ is PD  
> - Hyperbola otherwise  

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