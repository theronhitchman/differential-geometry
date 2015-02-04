---
layout: post
title: Hitchman Takes a Turn

---

Today Emily asked me to show how I start to think about one of these tasks.
There is value in watching an "expert" figure stuff out, so I did it.
The task in question was exercise 1.2.10 from Shifrin. This ended up taking the whole hour, so we didn't do anything else. I'll put a copy of my "solution" below, but it doesn't have the thinking part in it.

To help out with the thinking parts:

  * What examples do I know that I can model my understanding on? (In this
    case it was easy to pick out our canonical helix.)
  * How can I use the Frenet-Serret equations to make progress? Is there a
    differential equation nearby that I can use to my benefit?
  * When stuck, take a derivative.
  * In "theoretical" setups, it almost always helps to assume your curve is
    parameterized by arclength.

**I want to talk about project ideas!** look through the lists on the web page, think about what you might want to study. Come talk to me to sort it out. It is time to get moving on those.

**It is time to write up some solutions!** We haven't talked about this enough. See the grading table for "motivation."

----

### Solution to Shifrin 1.2.10

#### Exercise 1.2.10
Prove that if $\kappa = \kappa_0$ and $\tau = \tau_0$ are non-zero constants, then the curve is a (right) circular helix.


#### Solution
Without loss of generality, we assume that $\alpha$ is parametrized by arclength. Frenet's equation for $N$ tells us that  $N' = -\kappa_0 T + \tau_0 B$. We differentiate this to find:
\begin{align*}
N'' & = -\kappa_0 T' + \tau_0 B' \\
	& = -\kappa_0 (\kappa_0 N) + \tau_0 (-\tau_0 N) \\
	& = -(\kappa_0^2 + \tau_0^2 ) N .
\end{align*}
This means that $N$ satisfies the second order differential equation $N'' + k^2 N = 0$, where $k = \sqrt{(\kappa_0^2 + \tau_0^2 )}$. This is a simple harmonic oscillator equation, and its solutions are combinations of $\cos(k s)$ and $\sin(k s)$. Therefore, for some appropriate choice of vectors $v$ and $w$, we have
\[
\alpha''(s) = \kappa_0 N(s) = \kappa_0 \cos(ks) v + \kappa_0 \sin(ks) w .
\]
We integrate this twice to find that there are constant vectors $c$ and $b$ such that
\[
\alpha(s) = -\dfrac{\kappa_0}{k^2}\left( \cos(ks) v + \sin(ks) w \right) + s c + b .
\]
We now check that this is indeed a right circular helix. We want to show that the vectors $v, w$ are an orthonormal set and that $c$ is orthogonal to both $v$ and $w$. If this is the case, then our curve is a helix that has been hit with a rigid motion. The key fact is that $||N|| = 1$. Thus,
\[
1 = ||N||^2 = \cos^2(ks) ||v||^2 + \sin^2(ks) ||w||^2 + 2 \cos(ks)\sin(ks) v\cdot w.
\]
At $s=0$ we deduce that $1 = ||v||^2$. At $s = \pi/2k$, we deduce that $1 = ||w||$. Thus $v$ and $w$ are unit vectors. Putting this back into the equation above, we find that $1 = 1 + 2\cos(ks)\sin(ks) v\cdot w$.
This is only possible when $v\cdot w = 0$, so $v$ and $w$ are orthogonal. To see that $c$ is orthogonal to $v$ and $w$, we proceed similarly, based on the fact that $\alpha'$ and $N$ should be orthogonal. Using what we already know, we find  $0 = \alpha' \cdot N = \dots = \cos(ks) c\cdot v + \sin(ks) c \cdot w.$ So, again choosing special values of $s$ we get the conclusion.
