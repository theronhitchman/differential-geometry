---
layout: post
title: Parallels between curve theory and surface theory
---

Today Mark did Shifrin 2.3\#5.

Then I talked a lot about how the theory fits together. There were two main points:

  1. The First Fundamental Form is a type of thing called an "inner product" on
    the \\(uv\\)-plane. It is kinda like the dot product, because it has similar
    properties. In fact, it IS the dot product _from another space._ Recall that
    on a surface the tangent plane at a point is made up of those vectors in 3-space
    which are tangent to the surface at that point. This means we can express them
    as column vectors with three entries, and we can use the usual dot product in
    \\(\mathbb{R}^3\\) on them. But the tangent plane also has \\(x_u, x_v\\) as
    a basis. Which means we can represent a tanget vector as a vector with only
    two coordinates, too: \\(w = a x_u + b x_v \\approx (a,b) \\). This identification
    allows us to "pull-back" the dot product from 3-space to a kind of function
    on vectors in the \\(uv\\) plane. That new function is exactly described by the
    functions \\(E, F, G\\) and the matrix of the First Fundamental Form.
    (You did this computation as a homework exercise earlier in the term.)

  2. There is a way to organize what we have done so far that shows off the parallels
    between curve theory and surface theory.
    In curve theory, we found the Frenet framing \\(\\{T, N, B\\}\\) and then the
    curvature \\(\\kappa\\) shows off how the tangent moves (looking at second
    derivatives). Next, we look at how the normal directions move. This gives us
    \\(\\tau\\). (Note that we magically get away with one number to measure
    the tangential and normal components of the motion of N and B.)
    And finally then we derived some compatibility relations called the
    Frenet-Serret equations which come from looking at deeper derivatives.

    For surfaces, the tangent vector is replaced by the pair \\(x_u, x_v\\). That is the
    tangent information (given by first derivatives). Things are more complicated
    because there are two vectors. Rather than normalize by arclength, all we can do
    is track the first fundamental form.
    Then to study curvatures, we take another level of derivative. If we take the
    normal components of the second derivatives, we get curvature information
    (this is stuff in the second fundamental form, the shape operator, etc).
    Now, we can also look for the tangential components of the changes in
    \\(x_u, x_v\\) (that is, look at tangential components of second derivatives)
    and get Christoffel symbols.
    Finally, when we look at deeper derivatives, we will get compatibility relations.
    These relations are called the Gauss-Weingarten and Codazzi-Mainardi equations.

Nice and tidy, huh?
