---
title:
- Assignment 4 report for MIN E 612
author:
- Átila Saraiva Quintela Soares
date:
- \today
---

Code to generate the results can be found on the github repository [https://github.com/AtilaSaraiva/learning_variogram_and_stuff](https://github.com/AtilaSaraiva/learning_variogram_and_stuff/blob/fff8841c758a461fbd223c40c46c5b8fea1df236/src/assingment.ipynb)

# Question 1

By analysing the variogram map, the major direction of continuity is $N45^o$ and the minor is the minor is $N315^o$, perpendicular to the major direction.

Figure 1 shows the experimental variogram plot for the major and minor directions.

![Experimental variogram plot from the values in the variogram map](../../figs/assignment5-experimental.pdf)

In order to make the model for each direction, the gaussian function was chosen since the variograms have low values for small
lags. The function ended up being

$$\gamma_{major}(h) = 0.1042 + 0.2883\,Gauss(h, a=35) + 0.2998\,Gauss(h, a=50) + 0.3077\,Gauss(h, a=60)$$

$$\gamma_{minor}(h) = 0.1136 + 0.2935\,Gauss(h, a=20) + 0.2935\,Gauss(h, a=20) + 0.2995\,Gauss(h, a=50)$$

Figure 2 shows a plot of the modeled variogram versus the experimental variogram values.

![Modeled variogram plot from the values in the variogram map](../../figs/assignment5-modeled.pdf)

# Question 2

The calculated values for the moment of inertia were:

$I_{xx}=34, I_yy=54, I_xy=-288$

and

$\theta = {-44^o, 46}$
