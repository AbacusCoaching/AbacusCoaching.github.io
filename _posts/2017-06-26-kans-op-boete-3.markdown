---
layout: post
title:  "Onbetaald parkeren 3"
date:   2017-06-26 12:25:00 +0200
tags: [statistiek,parkeren,boete,poisson]
---
In de vorige 2 blogposts hadden we het al over parkeren zonder te betalen. Je weet dat de parkeerwachters 1 keer per uur langskomen en je wagen parkeerde je   gedurende 1 uur.

Maar wat moet je doen als je de frequentie van de parkeerwachters uitgedrukt wordt per uur en je parkeert maar voor een half uur? Want om de vorige berekenen te kunnen herhalen moet de parkeerduur overeen komen met de frequentie van de parkeerwachter en dit is nu niet het geval (half uur vs 1 uur).

De poisson verdeling heeft een hele mooie eigenschap: als je de frequentie met een factor a vermenigvuldigt, dan mag je het gemiddelde met diezelfde factor a vermenigvuldigen!

In dit concreet geval: de frequentie van de parkeerwachter is 1 keer per uur. Dit moet herleid worden naar een half uur. Dit kan door de frequentie met 0.5 te vermenigvuldigen. Dan komt de parkeerwachter gemiddeld 1*0.5 = 0.5 keer langs per half uur. Dit klinkt logisch, toch?

Nu kunnen we dezelfde berekeningen doen, maar nu is lambda gelijk aan 0.5.

$$
\begin{array}{rcl}
\\P(geen boete)&=&P(X=0) \\\\
&=&\frac{e^{-\lambda}\lambda^x}{x!}\\\\
&=&\frac{e^{-0.5}0.5^0}{0!}\\\\
&=&\frac{1}{\sqrt{e}}\\\\
&=&0.606530659712633
\end{array}
$$

De kans op geen boete is dus afgerond 61%. Maar dat betekent dus dat je 39% kans hebt op wel een boete, dus ongeveer 2 keer op 5.

Opgelet: dit resultaat mag je dus niet vergelijken met de eerste blogpost: daar parkeer je gedurende een volledig uur, in dit geval een half uur. Je moet dus telkens het volledige plaatje zien!