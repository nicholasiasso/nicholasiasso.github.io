<script type="text/javascript" async src="https://cdnjs.cloudflare.com/ajax/libs/mathjax/2.7.2/MathJax.js?config=TeX-MML-AM_CHTML"> </script> 

# The Bifurcation Diagram

Welcome to my first post! I wanted to show the math and code behind the following fractal, called the bifurcation diagram.

![Periodicity of rx(1-x)](..\assets\bifurcation\BifurcationDiagramSmoothColored.png)

## The Logistic Map

The bifurcation diagram is really an illustration of a concept called **Period Doubling**. This is a phenomenon which occurs in nature in countless ways, including the dripping of water, flowing of fluids, electrical circuits, and population sizes.


The basis of this fractal is a simple equation, called the logistic map, although many functions exhibit the same period doubling trait. We'll explore the logistic map here, as it's one of the simplest to understand.

$$ x_{n+1} = rx_{n}(1-x_{n}) $$

The logistic map is often explained as a way to model the population of animals over time. \(x_{n+1}\) represents the population of a species next year and it is calculated by multiplying some reproduction rate $r$ by the population in the previous year, times one minus the previous population. 

$rx$ accounts for some large number of organisms reproducing and bringing the population up, fighting against $1-x$, which represents a population running out of resources in it's ecosystem.

This function is just an upside-down parabola with fixed points at $(0, 0)$ and $(1, 0)$ for any $r$.

<iframe src="https://www.desmos.com/calculator/3bmn8i0kbm?embed" width="500" height="500" style="border: 1px solid #ccc" frameborder=0></iframe>

What's really interesting, is what happens over a long period of time. If we set $r$ to a constant value between $0$ and $4$, we can see many different patterns emerge after iterating for a long time.

Let's start on the low end, with $r=0.5$. When we iterate this, we can see that the population only ever declines, and after long enough, will fall to $0$. The same will apply for all values $0>r>1$.

After $1$, the function will tend to stabalize at some fixed value, no matter what we $x_{0}$ we start with.

This same behavior applies all the way up until about $3.45$, where we see something interesting happen. Instead of stabalizing at one value, it starts to stabalize towards two values, forever oscillating between them. This is also a stable attractor, meaning that for any value we start with, we will tend towards this pattern.

If we keep going, we will see this happen again: each of the stable points will split again in two, resulting in an oscillation with period $4$.

This pattern of the stable points each splitting into two continues. If we keep increasing $r$, we will see the four points split into eight, and then the eight points split into sixteen, and so on.

## The Feigenbaum Constant

So how much do we have to increase $r$ before the period splits again? A physicist named Mitchell J. Feigenbaum studied this behavior, and in 1975, discovered that the intervals between bifurcation points tend towards being $4.6692...$ times longer than the next. This value, commonly written as δ (delta), seems to be some foundational constant in methematics.

## Geometric Series

## Chaos

