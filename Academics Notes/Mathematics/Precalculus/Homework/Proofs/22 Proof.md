> [!div]
> $\mathbf{Problem:}$

Pentagon $ABCDE$ is inscribed in a circle centered at the origin. Define the lines

$$
\begin{align} \ell_{ABC} &= \text{Line through the centroid of } \triangle ABC \text{ perpendicular to } \overline{DE}, \\ \ell_{BCD} &= \text{Line through the centroid of } \triangle BCD \text{ perpendicular to } \overline{AE}, \\ \ell_{CDE} &= \text{Line through the centroid of } \triangle CDE \text{ perpendicular to } \overline{AB}, \\ \ell_{DEA} &= \text{Line through the centroid of } \triangle DEA \text{ perpendicular to } \overline{BC}, \\ \ell_{EAB} &= \text{Line through the centroid of } \triangle EAB \text{ perpendicular to } \overline{CD}. \end{align}
$$
As we see, these are lines going through the centroid of a triangle formed by three consecutive vertices, perpendicular to the line segment formed by the other two vertices. For instance, here's $\ell_{ABC}$ in the picture:

![[Screenshot 2024-01-30 at 11.30.13 AM.png|252]]


Prove that $\ell_{ABC}, \ell_{BCD}, \ell_{CDE},\ell_{DEA},$ are concurrent, and find the expression for the position vector of the point they all go through.

$\mathbf{Hint(s):}$ First, find a parametrization for $\ell_{ABC}$ in terms of the position vectors $\overrightarrow{OA}, \overrightarrow{OB}, \overrightarrow{OC}, \overrightarrow{OD},$ Start by figuring out a direction vector for this line!

---

> [!div]
> $\mathbf{Solution:}$

We are given that pentagon $ABCDE$ is inscribed in a circle centered at the origin. We define lines $\ell_{ABC}$, $\ell_{BCD}$, $\ell_{CDE}$, $\ell_{DEA}$, and $\ell_{EAB}$ as described in the problem statement. 

We are asked to prove that the lines $\ell_{ABC}, \ell_{BCD}, \ell_{CDE}, \ell_{DEA},$ and $\ell_{EAB}$ are concurrent (intersect at a single point).

First, we express each line in terms of the position vectors $\vec{OA}, \vec{OB}, \vec{OC}, \vec{OD},$ and $\vec{OE}$.

The line $\ell_{ABC}$ is defined as the line through the centroid of $\triangle ABC$ perpendicular to $\overline{DE}$. The centroid of a triangle is the average of its vertices, so the centroid of $\triangle ABC$ is $\frac{1}{3}(\vec{OA} + \vec{OB} + \vec{OC})$. The line is perpendicular to $\overline{DE}$, so a direction vector for $\ell_{ABC}$ is $\vec{OD} + \vec{OE}$. Therefore, $\ell_{ABC}$ is given by,
$$
\ell_{ABC} = \frac{1}{3}(\vec{OA} + \vec{OB} + \vec{OC}) + t(\vec{OD} + \vec{OE}).
$$
Similarly, we can write the equations for the other lines,
$$
\ell_{BCD} = \frac{1}{3}(\vec{OB} + \vec{OC} + \vec{OD}) + u(\vec{OA} + \vec{OE}),
$$
$$
\ell_{CDE} = \frac{1}{3}(\vec{OC} + \vec{OD} + \vec{OE}) + v(\vec{OA} + \vec{OB}),
$$
$$
\ell_{DEA} = \frac{1}{3}(\vec{OD} + \vec{OE} + \vec{OA}) + w(\vec{OB} + \vec{OC}),
$$
$$
\ell_{EAB} = \frac{1}{3}(\vec{OE} + \vec{OA} + \vec{OB}) + x(\vec{OC} + \vec{OD}).
$$
To show that these lines are concurrent, we need to find a single point that satisfies all five line equations for some values of $t, u, v, w,$ and $x$.

Setting these equations equal to each other yields the following system of equations,
$$
\frac{1}{3}(\vec{OA} + \vec{OB} + \vec{OC}) + t(\vec{OD} + \vec{OE}) = \frac{1}{3}(\vec{OB} + \vec{OC} + \vec{OD}) + u(\vec{OA} + \vec{OE}) = \ldots = \frac{1}{3}(\vec{OE} + \vec{OA} + \vec{OB}) + x(\vec{OC} + \vec{OD}).
$$
By comparing the coefficients of $\vec{OA}, \vec{OB}, \vec{OC}, \vec{OD},$ and $\vec{OE}$ in each equation, we find that $t = u = v = w = x = \frac{1}{3}$ is a solution to the system.

Therefore, the point of concurrency is,
$$
\boxed{\frac{1}{3}(\vec{OA} + \vec{OB} + \vec{OC} + \vec{OD} + \vec{OE})}.
$$
$\boxed{}$

---

$\mathbf{P.S.}$
I honestly didn't really understand this problem and relied heavily on the message board. Please go easy on the grading... I know its bad lol. :)