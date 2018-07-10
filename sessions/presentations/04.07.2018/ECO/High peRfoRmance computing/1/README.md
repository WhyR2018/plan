# Tricks for faster R code

[Tomasz	Melcer,	QuantUp]()

## Description

Unless we are working with very small datasets, computation time is something that slows down analytics of any kind, whether business-related or academic. We usually need to run analyses many times, and if data processing takes more than a short while, human mind starts to wander off and we get less efficient. To waste less time on waiting for results, we may attempt to make our code faster. This is, however, a trade-off: optimizing code takes human time too! I will talk about some tricks that can speed up code with little effort: memoization and parallelization. I will show some common cases where these techniques bring most benefits, but also discuss when to avoid them.

