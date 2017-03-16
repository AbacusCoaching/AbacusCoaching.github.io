---
layout: post
title:  "Rollercoaster defect"
date:   2014-07-10 03:40:45 +0200
categories: statistiek  poisson  bobbejaanland  rollercoaster
---
De Typhoon  in Bobbejaanland viel voor de tweede keer in panne volgens [dit bericht in het nieuwsblad](http://www.nieuwsblad.be/article/detail.aspx?articleid=dmf20140708_01171415). Maar hoe uitzonderlijk is dit nu?

Het aantal gebeurtenissen in een tijdsinterval worden typisch gemodeleerd door een poison distributie. Als de rollercoaster 1 keer per jaar defect is, dan is het aantal defecten per jaar een poisson proces met gemiddelde 1 defect/jaar. Om het aantal defecten per week voor te stellen, moet je het gemiddelde proportioneel aanpassen. In dit geval is het gemiddelde lambda gelijk aan 1 defect/52 weken.

Nu kunnen we de kans berekenen op 2 defecten in 1 week. Stel X het aantal defecten per week, dan zoeken we P(X=2).

$$
\begin{array}{rcl}
P(X=x)&=&\frac{\lambda^x\exp(-\lambda)}{x!}\\\\
P(X=2)&=&\frac{(1/52)^2\exp(-(1/52)}{2!}\\\\
&=&0.000181389231205673
\end{array}
$$

De kans op 2 defecten in 1 week is dus 0.000181389231205673. De persverantwoordelijke heeft dus zeker gelijk als hij zegt dat dit uitzonderlijk is.
