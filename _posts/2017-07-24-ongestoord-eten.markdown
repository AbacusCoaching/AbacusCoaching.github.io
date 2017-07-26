---
layout: post
title:  "Ongestoord eten"
date:   2017-07-24 20:54:00 +0200
tags: [statistiek,eten,poisson]
---
Na een lange, vermoeiende werkdag wil je ongestoord eten in de stad. Je trekt hiervoor 2 uur uit en je wil tijdens deze 2 uur geen enkele kennis tegen het lijf lopen. Telkens je naar de stad gaat kom je 2 bekenden per uur tegen het lijf. Wat is de kans dat je wens werkelijkheid wordt?


De toevalsvariabele X is het aantal bekenden die je in 2 uur tegenkomt. Dit is -opnieuw- een voorbeeld van de poisson verdeling.

Een eigenschap van poisson is dat het gemiddelde evenredig is het tijdsinterval. Dit betekent dat je in 2 uur gemiddeld 4 bekenden tegen het lijf loopt.
X is dus poisson verdeeld met lambda 4 (4 bekenden per 2 uur). De kans om ongestoord te kunnen eten:


$$
\begin{array}{rcl}
\\P(0 bekenden)&=&P(X=0) \\\\
&=&\frac{e^{-\lambda}\lambda^x}{x!}\\\\
&=&\frac{e^{-4}4^0}{0!}\\\\
&=&\frac{1}{e^4}\\\\
&=&0.01831563888873
\end{array}
$$

Het is dus zeer onwaarschijnlijk om in alle rust je maaltijd te verorberen.
