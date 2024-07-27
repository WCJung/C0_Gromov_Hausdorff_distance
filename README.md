# C0_Gromov_Hausdorff_distance

This repository is the official implementation of in the submitted paper "Approximating real functions with varying domain".

The purpose of README.md is to introduce the original concept of the $C^0$-Gromov-Hausdorff distance for compact metric spaces [1]. We study on finite metric spaces from an approximation perspective and discuss its application to neural networks, which can be found in the submitted paper.


One of motivation behind this work [1] is to provide an understanding of the classical Gromov-Hausdorff metric [2] by extending it to maps between metric spaces. The following definition of Gromov-Hausdorff distance which is equivalent to the approach in [2].

Consider a metric space $X$, given $A,B \subset X$ we define the hausdorff distance between $A$ and $B$.

$$d_H(A,B) = \max \\{ \sup_{a \in A} d(a,B), \sup_{b \in B} d(A,b) \\}.$$

An isometry between the metric spaces $X$ and $Y$ is an onto map $i : X \to Y$ satisfying $d(i(x),i(x')) = d(x,x')$ for every $x, x' \in X$, We say that $X$ and $Y$ are isometric if such an isometry exists.

Given $\Delta >0$, a (noncecessarily continuous and onto) map $i : X \to Y$ between the metric space $X$ and $Y$ is called $\Delta-isometry$ if

$$ \max \\{ d_H(i(X),Y), \sup_{x, x' \in X} |d(f(x),f(x') - d(x,x')| \\} < \Delta.$$

The Gromov-Hausorff distance between the metric spaces $X$ and $Y$ is defined by

$$d_{GH}(X,Y) = \inf \\{ \Delta > 0 : \exists \Delta-isometry \: i : X \to Y and j : Y \to X   \\} . $$

Here, we recall the classical $C^0$ distance between the maps $f : X \to X$ and $g : X \to X$ of the same metric space $X$ defined by

$d_{C^0}(f,g) = \sup_{x \in X} d(f(x),g(x))$.

A slight modification of the Gromov-Hausdorff distance including the $C^0$ distance above yields the following definition. We define the $C^0$-Gromov-Hausdorff distance between maps $f:X \to X$ and $g :Y \to Y$ of the metric spaces $X$ and $Y$, respectively.

$$d_{GH^0}(f,g) = \inf \\{ \Delta > 0 : \exists \Delta-isometry i : X \to Y and j : Y \to X such that d_{C^0}(g \circ i, i \circ f) and d_{C^0}(j \circ g, f \circ j) \\}. $$




## References

[1] A. Arbeito, C. A. Morales, *Topological stability from Gromov-Hausdorff viewpoint*, Discrete and Continuous Dynamical Systems 37 (2017), no. 7, 3531–3544.

[2] M. Gromov, *Metric Structures for Riemannian and Non-Riemannian Spaces*, Based on the 1981 French original. With appendices by M. Katz, P. Pansu and S. Semmes. Translated from the French by Sean Michael Bates. Progress in Mathematics, 152. Birkhäuser Boston, Inc. , Boston, MA, 1999.
