---
layout: post
title:  "Ongestoord eten 2"
date:   2017-07-31 18:34:00 +0200
tags: [statistiek,eten,poisson]
---
In de vorige blokpost werd de kans berekend om ongestoord te eten in de stad. Een alternatieve manier is gebruik maken
van de wachttijd tussen 2 opeenvolgende gebeurtenissen?

_Que?_ Poisson wordt gebruikt om vooral gebeurtenissen in een tijdsinterval voor te stellen. Een eigenschap van poisson
is dat de wachttijd tussen __2 opeenvolgende__ gebeurtenissen exponentieel verdeeld is met als parameter het gemiddelde van
poisson. In het diner voorbeeld was het gemiddelde is 2 bekenden per uur. Dus de wachttijd tussen 2 opeenvolgende
gebeurtenissen is exponentieel verdeeld met gemiddelde 2.

Nu kunnen we berekenen wat de kans is dat de wachttijd tussen 2 opeenvolgende gebeurtenissen minstens 2 uur is. Noem de wachttijd X en dan heb je volgende berekeningen:

$$
\begin{array}{rcl}
\\P(X>t)&=&e^{-\lambda t}\\\\
&=&e^{-2*2}\\\\
&=&\frac{1}{e^4}\\\\
&=&0.01831563888873
\end{array}
$$

Via een andere weg wordt hetzelfde resultaat bekomen - typisch wiskunde :)
