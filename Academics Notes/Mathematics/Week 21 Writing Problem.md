$\mathbf{Problem:}$
Let $\ell$ be the set of all points $(x,y,z)$ such that
$$
\begin{pmatrix} x\\ y \\ z \end{pmatrix} = \begin{pmatrix} 0 \\ 1 \\ 2 \end{pmatrix} + t \begin{pmatrix} 1\\2 \\3 \end{pmatrix}
$$
for some real $t$, and let $P$ be the plane with equation
$$
x+y+z = 1.
$$
(a) Prove that the matrix
$$
\mathbf{A} =  \begin{pmatrix} -2 & -2 & 2 \\ 2 & 0 & 1 \\ 0& -1 & -1 \end{pmatrix}
$$
maps all points on line $\ell$ to points on plane $P$.

(b) Prove that the matrix
$$
\mathbf{B} =  \begin{pmatrix} 1 & 1 & -1 \\ 3 & 3 & -1 \\ 5& 5 & -1 \end{pmatrix}
$$
maps all points on plane $P$ to points on line $\ell$.


---

$\mathbf{Solution:}$
$\mathbf{a)}$

To prove that matrix $\mathbf{A}$ maps every point on the parametrized line $\ell$ onto a plane with an equation of $x+y+z=1$, we must take a generalized approach.

Keeping our parametrization generalized, we treat $t$ as an arbitrary variable and solve to obtain,
$$
\begin{aligned}
\begin{pmatrix}
x \\ y \\ z 
\end{pmatrix} &= \begin{pmatrix}
0 \\ 1 \\ 2
\end{pmatrix} + \begin{pmatrix}
t \\ 2t \\3t
\end{pmatrix} \\
&= \begin{pmatrix}
t \\ 2t+1 \\ 3t+2
\end{pmatrix}.
\end{aligned}
$$
We may now proceed with applying matrix $\mathbf{A}$ to this vector to verify that it does indeed map our parametrized point to plane $P$. 
$$
\begin{aligned}
\mathbf{A} \begin{pmatrix}
t \\ 2t+1 \\ 3t+2
\end{pmatrix} &= \begin{pmatrix}
-2 & -2 & 2 \\ 2 & 0 & 1 \\ 0 & -1 & -1
\end{pmatrix} \begin{pmatrix}
t  \\
2t+1 \\
3t+2
\end{pmatrix} \\
&=  \begin{pmatrix}
-2t-2(2t+1)+2(3t+2) \\
2t+0(2t+1)+1(3t+2) \\
0t-1(2t+1)-1(3t+2)
\end{pmatrix} = \boxed{ \begin{pmatrix}
2 \\
5t+2 \\
-5t-3
\end{pmatrix}}.
\end{aligned}
$$

Summing the $x$, $y$, $z$ components of our transformed vector yields the desired result,
$$
2+5t+2-5t-3=1.
$$
Thus, we have proven that matrix $\mathbf{A}$, in fact, does map all points on the parametrized line $\ell$ onto plane $P$.

$\boxed{}$

-----

$\mathbf{b)}$

To prove that matrix $\mathbf{B}$ sends any point on plane $P$ to our parametrized line $\ell$, we must again take a generalized approach.

We begin by using $\begin{pmatrix} s \\ n \\ 1-s-n \end{pmatrix}$ to represent a random point on plane $P$, as the sum of its components is equal to $1$.

Applying matrix $\mathbf{B}$ to this point yields,
$$
\begin{aligned}
\mathbf{B} \begin{pmatrix}
s \\ n \\ 1-s-n
\end{pmatrix} &= \begin{pmatrix}
1 & 1 & -1 \\ 3 & 3 & -1 \\ 5 & 5 & -1
\end{pmatrix} \begin{pmatrix}
s  \\
n \\
1-s-n
\end{pmatrix} \\
&= \begin{pmatrix}
s + n - (1-s-n) \\
3s + 3n - (1-s-n) \\
5s + 5n - (1-s-n)
\end{pmatrix} = \boxed{ \begin{pmatrix}
2s + 2n - 1 \\
4s + 4n - 1 \\
6s + 6n -1
\end{pmatrix}}.
\end{aligned}
$$
This vector can be decomposed into
$$
\begin{pmatrix}
-1 \\
-1 \\
-1
\end{pmatrix}+t\begin{pmatrix}
1 \\
2 \\
3
\end{pmatrix}
$$
where $t=2n+2s$.

Thus, the translated points direction vector is proportional to our parametrized equation's direction vector. Although this does describe parametrization $\ell$, a discrepancy exists between the two position vectors. Luckily, we are allowed to change the position vector by adding multiples of the direction vector to the equation.

It is clear that we only need to add one multiple of the direction vector to our equation to eliminate the discrepancy,
$$
\begin{pmatrix}
-1 \\
-1 \\
-1
\end{pmatrix}
+ \begin{pmatrix}
1 \\
2 \\
3 \\
\end{pmatrix}
+t 
\begin{pmatrix}
1 \\
2 \\
3
\end{pmatrix}
= \boxed{\begin{pmatrix}
0 \\
1 \\
2 \\
\end{pmatrix}
+ t\begin{pmatrix}
1 \\
2 \\
3
\end{pmatrix}}.
$$
Therefore, we have demonstrated that matrix $\mathbf{B}$ maps any point on plane $P$ onto the parametrized line $\ell$.

$\boxed{}$
<br>
[Precalculus Week 21 Problem 13 | Desmos](https://www.desmos.com/3d/00194811ff)