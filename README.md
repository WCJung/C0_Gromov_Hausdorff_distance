# C0_Gromov_Hausdorff_distance

In paper [1], one of motivation behind this work is to provide an understanding of the classical Gromov-Hausdorff metric [2] by extending it to maps between metric spaces. First, the following definition of Gromov-Hausdorff distance from [1], which is equivalent to the approach in [2].

Consider a metric space $X$, given $A,B \subset X$ we define the hausdorff distance between $A$ and $B$.

$$d_H(A,B) = \max \left{ \sup_{a \in A} d(a,B), \sup_{b \in B} d(A,b) \right}.$$

An isometry between the metric spaces $X$ and $Y$ is an onto map $i : X \to Y$ satisfying $d(i(x),i(x')) = d(x,x')$ for every $x, x' \in X$, We say that $X$ and $Y$ are isometric if such an isometry exists.

Given $\Delta >0$, a (noncecessarily continuous and onto) map $i : X \to Y$ between the metric space $X$ and $Y$ is called $\Delta-isometry$ if

$$ \max \left{ d_H(i(X),Y), \sup_{x, x' \in X} |d(f(x),f(x') - d(x,x')| \right} < \Delta.$$

The Gromov-Hausorff distance between the metric spaces $X$ and $Y$ is defined by

$$d_{GH}(X,Y) = \inf \left{ \Delta > 0 : \exists \Delta \mbox{-isometry) \: i : X \to Y \: \mbox{and} \: j : Y \to X   \right} . $$

Here, we recall the classical $C^0$ distance between the maps $f : X \to X$ and $g : X \to X$ of the same metric space $X$ defined by

$d_{C^0}(f,g) = \sup_{x \in X} d(f(x),g(x))$.

A slight modification of the Gromov-Hausdorff distance including the $C^0$ distance above yields the following definition. We define the $C^0$-Gromov-Hausdorff distance between maps $f:X \to X$ and $g :Y \to Y$ of the metric spaces $X$ and $Y$, respectively.

$$d_{GH^0}(f,g) = \inf \left{ \Delta > 0 : \exists \Delta \mbox{-isometry) \: i : X \to Y \: \mbox{and} \: j : Y \to X  such that d_{C^0}(g \circ i, i \circ f) \: \mbox{and} \: d_{C^0}(j \circ g, f \circ j) \right} . $$


## References

[1] A. Arbeito, C. A. Morales, *Topological stability from Gromov-Hausdorff viewpoint*, Discrete Contin. Dyn. Syst. 37 (2017), no. 7, 3531–3544.

[2] M. Gromov, Metric Structures for Riemannian and Non-Riemannian Spaces, Based on the 1981 French original. With appendices by M. Katz, P. Pansu and S. Semmes. Translated from the French by Sean Michael Bates. Progress in Mathematics, 152. Birkhäuser Boston, Inc. , Boston, MA, 1999.

[3] P. Walters, On the pseudo-orbit tracing property and its relationship to stability, The structure of attractors in dynamical systems (Proc. Conf. , North Dakota State Univ. , Fargo, N. D. , 1977), Lecture Notes in Math. , Springer, Berlin, 668 (1978), 231-244.

[4] Chazal, F., Cohen-Steiner, D., Guibas, L.J., M´emoli, F. Oudot, S.Y., Gromov-Hausdorff stable signatures for shapes using persistence, Computer Graphics Forum, 28 (2009), 1393–1403.
