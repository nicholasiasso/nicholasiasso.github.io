# The Bifurcation Diagram

Welcome to my first post! In the first post here, I'll explain the math and code behind the following fractal, called the bifurcation diagram.

![Periodicity of rx(1-x)](..\assets\bifurcation\BifurcationDiagramSmoothColored.png)

## The Logistic Map

The bifurcation diagram is really an illustration of a concept called **Period Doubling**. This is a phenomenon which occurs in nature in countless ways, including the dripping of water, flowing of fluids, electrical circuits, and population sizes.


The basis of this fractal is a simple equation, called the logistic map, although many functions exhibit the same period doubling trait. We'll explore this the logistic map here, as it's one of the simplest to understand.

$$ f(x_{n+1}) = rx_{n}(1-x_{n}) $$

This function is just an upside-down parabola with fixed points at $(0, 0)$ and $(1, 0)$ for any $r$.

<iframe src="https://www.desmos.com/calculator/3bmn8i0kbm?embed" width="500" height="500" style="border: 1px solid #ccc" frameborder=0></iframe>

