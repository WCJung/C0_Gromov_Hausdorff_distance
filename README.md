# C0_Gromov_Hausdorff_distance

In paper [1], one of motivation behind this work is to provide an understanding of the classical Gromov-Hausdorff metric [2] by extending it to maps between metric spaces. First, the following definition of Gromov-Hausdorff distance from [1], which is equivalent to the approach in [2].

Consider a metric space $X$, given $A,B \subset X$ we define the hausdorff distance between $A$ and $B$.

$$d_H(A,B) = \max { \sup_{a \in A} d(a,B), \sup_{b \in B} d(A,b) }.$$

An isometry between the metric spaces $X$ and $Y$ is an onto map $i : X \to Y$ satisfying $d(i(x),i(x')) = d(x,x')$ for every $x, x' \in X$, We say that $X$ and $Y$ are isometric if such an isometry exists.

Given $\Delta >0$, a (noncecessarily continuous and onto) map $i : X \to Y$ between the metric space $X$ and $Y$ is called $\Delta-isometry$ if

$$ \max { d_H(i(X),Y), \sup_{x, x' \in X} |d(f(x),f(x') - d(x,x')| } < \Delta.$$




## References

[1] A. Arbeito, C. A. Morales, *Topological stability from Gromov-Hausdorff viewpoint*, Discrete Contin. Dyn. Syst. 37 (2017), no. 7, 3531–3544.

[2] M. Gromov, Metric Structures for Riemannian and Non-Riemannian Spaces, Based on the 1981 French original. With appendices by M. Katz, P. Pansu and S. Semmes. Translated from the French by Sean Michael Bates. Progress in Mathematics, 152. Birkhäuser Boston, Inc. , Boston, MA, 1999.

[3] P. Walters, On the pseudo-orbit tracing property and its relationship to stability, The structure of attractors in dynamical systems (Proc. Conf. , North Dakota State Univ. , Fargo, N. D. , 1977), Lecture Notes in Math. , Springer, Berlin, 668 (1978), 231-244.

[4] Chazal, F., Cohen-Steiner, D., Guibas, L.J., M´emoli, F. Oudot, S.Y., Gromov-Hausdorff stable signatures for shapes using persistence, Computer Graphics Forum, 28 (2009), 1393–1403.
