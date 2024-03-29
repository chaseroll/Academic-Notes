---
tags:
  - Physics
  - Classical-Mechanics
  - Kinematics
Related:
  - "[[01. Space, Position, Time, and the need for Measurements]]"
Contents:
  - "[[#Introduction]]"
  - "[[#Velocity]]"
---
# Introduction

In Renaissance Florence, young **[Galileo Galilei's](https://en.wikipedia.org/wiki/Galileo_Galilei)** curiosity is piqued by the motions of nature. As objects move, they sketch unseen lines through space and time, and Galileo is driven to uncover the fundamental truths behind these motions. He begins to craft the basic constructs of Displacement, Velocity, and Acceleration, laying the foundation stones of classical mechanics.

Remember, these notes are meant to serve as a memory refresh and include some ideas that YOU uncovered and found helpful. <span style = "color:var(--text-normal)">You SHOULD NOT be creating a textbook!!!</span> 

<iframe width="560" height="315" src="https://www.youtube.com/embed/ErMSHiQRnc8?si=sopsZwJYCS4R5fkP" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>


---

# Velocity  
> [!div]
> ### Definition / Conceptual Idea
>
The velocity of an object is the rate at which an object changes its position. The direction of an object's velocity at any time is parallel to the tangent vector of the curve representing the trajectory of the object.
> 
>  [Source](https://youtube.com) $\quad$ [Resource 1](https://youtube.com) $\quad$ [Resource 2](https://youtube.com)

From the definition, the derivative of the position function yields the velocity function: $$ \color{var(--text-normal)}v(t) = \frac{dx}{dt} = \lim_{\Delta t \to 0} \frac{x(t + \Delta t) - x(t)}{\Delta t} = \lim_{\Delta t \to 0} \frac{x_2 - x_1}{\Delta t}. $$
Often, the term <span style="font-weight:bold; color: var(--text-normal)" >speed</span> is used instead of velocity. <mark class="custom-highlight">The speed of an object is the norm of the velocity</mark>,  i.e. it gives the **[[magnitude]]** but not the direction of the velocity.
^definition-of-speed

The speed function is therefore,

$$ |\vec{v}(t)| = \left| \frac{dx}{dt} \right| = \left| \lim_{\Delta t \to 0} \frac{x(t + Δt) - x(t)}{\Delta t} \right|. $$

Since the velocity of a particle is the derivative of its position, we can go the other way around to get displacement by integrating the velocity function; that is,

$$\int v(t) = \int \frac{ds}{dt} = s(t) + C, $$
$$ x^2 + y^2 = r^2 $$

where C is an arbitrary constant which can be found out if we are given an initial value.



> [!div]
> ### Example
>
>  The displacement of an object at some given time $t$ is given by the function $x(t)=3t^2 - 2t - 1$. Find the function that gives its velocity at all times and evaluate for $t=3$ and  $t=5.$
>
>---
>
> Since the velocity is the derivative of the displacement function,
> 
>  $$ v(t) = \frac{d}{dt}(3t^2 - 2t - 1) = 6t - 2. $$
> 
> Therefore, the speed function will be $\color{var(--text-normal)}|v(t)| = |6t - 2|$. As a result, the velocity and speed at $\color{var(--text-normal)}t=3$ are
> 
> $$v(3) = 6(3) - 2 = 16 \text{ m/s}, \quad |v(3)| = |16| = 16 \text{ m/s}, $$
> 
>  and at $t=5$
> 
> $$ v(5) = 6(5) - 2 = 28 \text{ m/s}, \quad |v(5)| = |28| = 28 \text{ m/s}. $$
>  <span style="color:gray;">&#9633;</span>
> 
>  [Source](https://youtube.com) $\quad$ [Additional Examples](https://youtube.com)$\quad$ [Practice Problems](https://youtube.com)




