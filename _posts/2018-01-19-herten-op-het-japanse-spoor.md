---
layout: post
title:  "Herten op het Japanse spoor"
date:   2018-01-19 12:45:00 +0200
tags: [statistiek,herten,poisson]
---
Op [HLN.be](https://www.hln.be/bizar/de-treinen-doen-wat-japan-neemt-bizarre-maatregel-om-herten-te-verjagen~a005ac9b) vind je wel meer bizarre berichten. Dit is er een van.

In Japan rijden de treinen veel herten omver. Door te toeteren hebben ze dit teruggebracht tot 7.5 herten per 100 kilometer. De route van Kioto naar Tokyo is
is 457 km. Hoeveel kans is er dat je op de bestemming komt zonder dierenleed?

Dit is alweer een poisson proces, deze keer met gemiddeld 7.5/100km . Over een afstand van 457 kilometer wordt het gemiddelde dan 34,275 herten/457 km.
$$
\begin{array}{rcl}
\\P(0 herten)&=&P(X=0) \\\\
&=&\frac{e^{-\lambda}\lambda^x}{x!}\\\\
&=&\frac{e^{-34.275}34.275^0}{0!}\\\\
&=&0
\end{array}
$$

Met andere woorden: er wordt zeker minstens 1 hert aangereden!
