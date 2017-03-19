---
layout: post
title:  "Subway voor de rechter wegens te kleine broodjes?"
date:   2013-01-25 18:39:03 +0100
tags:  [statistiek,hypothese testen,subway]
---
In de metro van 25 januari 2013 stond een artikel met als titel 'Subway voor de rechter wegens te kleine broodjes'. Volgens 2 frequente bezoekers van de broodjeszaak zijn sandwiches systematisch te klein. Maar hoe bewijs je zoiets?

Zoals altijd helpt statistiek hier, meer bepaald het principe van hypothese testen. We willen testen of de gemiddelde lengte van de broodjes minstens een foot lang is. Als we ervan uit gaan dat er een foutmarge is van 1 centimeter, dan kunnen we stellen dat de lengte van de broodjes gemiddeld 30cm is met een standaard afwijking van 1 cm.

Als we een voldoende grote steekproef nemen, dwz minstens 25 broodjes, en we bestellen de broodjes in willekeurige winkels -dus niet altijd dezelfde-, dan is de centrale limietstelling van toepassing. Als we Li de lengte noemen van het i-de broodje, dan heeft Li als gemiddelde 30 en als standaard afwijking 1. Het steekproefgemiddelde van onderlinge, onafhankelijke metingen Li-vandaar de vereiste van willekeurige winkels- wordt dan benaderd door een normaalverdeling met gemiddelde 30 en variantie 1/n, met n het aantal gemeten broodjes, of wiskundig

$$L_i \sim N(30,1^2), i=1\ldots n \rightarrow \bar{L}=\frac{\sum_{i=1}^n L_i}{n} \sim N(30,\frac{1^2}{n})$$

De hypothese die we willen testen is dat de gemiddelde lengte van de broodjes minstens 30 cm zijn dus dit wordt:

$$H_0: \mu \ge 30 \leftrightarrow H_a: \mu \le 30$$

Dit is nu een typisch voorbeeld van eenzijdig testen. Stel nu dat de steekproefdata (29,26,28,30,31,29,26,24,27,26,25) is, dan wordt het steekproefgemiddelde:

$$ \bar{l}=\frac{29+26+28+30+31+29+26+24+27+26+25}{11}=\frac{301}{11} = 27.36 $$

Het steekproefgemiddelde is 27.36 cm, dus onder het verwacht gemiddelde van 30 cm, maar dit kan liggen aan de variantie van de lengte van de broodjes. Om zeker te zijn of het toevallig is of niet wordt de kans berekend dat het steekproefgemiddelde van een andere test een nog kleiner gemiddelde heeft.

$$
\begin{array}{rcl}
P(\bar{L}<27.36)&=&P(\frac{\bar{L}-30}{1/\sqrt{11}}<\frac{27.36-30}{1/\sqrt{11}})\\
&=&\Phi(-8.75)\\
&=&0
\end{array}
$$

Blijkbaar heb je geen enkele kans om een steekproefgemiddelde te bekomen dat nog kleiner is dan het resultaat van deze steekproef. Je kan de hypothese zeker verwerpen bij! Het ziet er dus naar uit dat beide klanten de rechtzaak zullen winnen.
