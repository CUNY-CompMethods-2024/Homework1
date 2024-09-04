# HW1 - Exercise 3.2: Curve plotting in Python: A refresher

Although the plot function is designed primarily for plotting standard xy graphs, it can be adapted for other kinds of plotting as well.

a) Using pyplot, make a plot of the so-called deltoid curve, which is defined parametrically by the equations, x = 2 cos(θ) + cos(2θ) and y = 2 sin(θ) − sin(2θ), where 0 ≤ θ < 2π. 
To do this, take a set of values of θ between zero and 2π, and calculate x and y for each from the equations above, then plot y as a function of x.

b)  Taking this approach a step further, one can make a polar plot r = f(θ) for some function f by calculating r for a range of values of θ and then converting r and θ to Cartesian coordinates using the standard equations x = r cos θ, y = r sin θ. Use this method to make a plot of the Galilean spiral, $$r=θ^2 $$ for 0 ≤ θ ≤ 10π.

c)  Using the same method, make a polar plot of “Fey’s function” in the range 0 ≤ θ ≤ 24π.
$$r = e^{\cos{\theta}} - 2 \cos{4 \theta} + \sin^5{\frac{\theta}{12}} $$ 

Put all 3 plots in one figure with labels making it clear which plot is which. If you're doing this with an ipython notebook, you can have the figure display inline. Otherwise, save the figure as a png or pdf file, and include it in your clone of this repository.
