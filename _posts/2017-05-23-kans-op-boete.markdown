---
layout: post
title:  "Onbetaald parkeren"
date:   2017-05-23 21:55:00 +0200
tags: [statistiek,parkeren,boete,poisson]
---
In alle grote steden wordt de auto meer en meer geweerd. Een gevolg is dat enkel betalend parkeren mogelijk is. Wat als je niet wilt betalen,
 wat is dan de kans op een boete?
 
Om het concreet te maken: je parkeert je wagen en een vriend met teveel tijd die in de buurt woont, weet je te vertellen dat er gemiddeld 1 
parkeerwachter per uur passeert. Wat is de kans dat je een boete krijgt als je een uur onbetaald parkeert?

Dit is een mooi voorbeeld van de Poisson verdeling. Deze beschijft de kans op aantal gebeurtenissen in een interval. Interval kan heel ruim
geinterpreteerd worden: 

* tijdsinterval: aantal passerende autos per uur, aantal stroomuitvallen per week, ... 
* oppervlakteinterval: aantal defecte chips per vierkante centimeter
* zelfs volumeinterval: aantal rozijnen per kubieke decimeter deeg

In dit geval spreken we over een tijdsinterval. De toevalsvariabele $X$ is het aantal parkeerwachters die je wagen controleren tijdens je uur onbetaald parkeren.
Poisson heeft 1 parameter $\lambda$, die is in dit geval 1 (1 parkeerwachter per uur).


$$
\begin{array}{rcl}
\\P(geen boete)2&=&P(X=0) \\\\
&=&\frac{e^{-\lambda}\lambda^x}{x!}\\\\
&=&\frac{e^{-1}1^0}{0!}\\\\
&=&\frac{1}{e}\\\\
&=&0.36787944117
\end{array}
$$

De kans op geen boete is dus afgerond 37%. Maar dat betekent dus dat je 63% kans hebt op wel een boete, dus ongeveer 2 keer op 3, dus nog altijd vrij groot.