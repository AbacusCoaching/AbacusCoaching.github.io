---
layout: post
title:  "Speelt iTunes willekeurig genoeg?"
date:   2012-08-06 11:55:05 +0200
tags: [statistiek,iTunes,hypothese testen]
---
Volgens een artikel op http://lifehacker.com/5929611/why-itunes-shuffle-isnt-random-and-how-to-fix-it zou iTunes niet zo  willekeurig werken als gedacht. Maar hoe kan je dit nu controleren? Met statistiek natuurlijk en meer bepaald met hypothese testen.

Veronderstel dat we een playlist hebben van 36 liedjes. Bij willekeurig afspelen heeft elk liedje een gelijke kans omgekozen te worden, hier dus 1/6. Als iTunes op willekeurig staat en 36 liedjes uit deze lijst worden geselecteerd, dan wordt verwacht dat elke nummer gemiddeld 6 keer gespeeld wordt. n=36 pogingen, p=1/6 kans op succes: een typisch voorbeeld van een binomiaal verdeling, en die heeft als gemiddelde n*p=36/6=6.

We kijken nu even wat het resultaat is van 36 liedjes spelen. We krijgen bv deze frequenties van de steekproef:

$$\underline{x}=(x_i)=(7;6;8;6;6;3),\sum_i x_i = 36$$

*Eerste stap* is het formuleren van de nullhypothese: iTunes speelt in een echt willekeurige volgorde liedjes af. Of wiskundig geschreven: het gemiddeld aantal keer dat elk liedje gekozen kan worden is 6. De alternatieve hypothese is de negatie: het gemiddeld aantal keer dat elk liedje gekozen kan worden is verschillend van 6
$$H_0: EX_i=6 \leftrightarrow H_a: EX_i \neq 6 $$

*Tweede stap* is de kans berekenen dat we dezelfde of 'grotere' steekproef kunnen bekomen. De exacte verdeling van de steekproef onder de nullhypothese is multinomiaal. Deze kans berekenen is zeer moeilijk, dus maken we gebruik van de Chi Square test met 5 vrijheidsgraden - http://en.wikipedia.org/wiki/Pearson%27s_chi-squared_test .

$$
\begin{array}{rcl}
\\chi^2&=&\sum_i\frac{(x_i-EX_i)^2}{EX_i} \\\\
&=&\frac{1}{6}\sum_i(x_i-6)^2\\\\
&=&\frac{1}{6}(1+0+4+0+0+9)\\\\
&=&\frac{14}{6}\\\\
&=&2.3333
\end{array}
$$

De kans dat een chi kwadraat variabele met 5 vrijheidsgraden groter is dan 2.3333 kan je online berekenen, bv bij deze Chi-Square Calculator - http://www.fourmilab.ch/rpkp/experiments/analysis/chiCalc.html

$$ P(\chi^2>2.3333)=0.1987$$

*Laatste stap* is het besluit formuleren. Uitgaande van een betrouwbaarheid van 90% kunnen we de nullhypothese niet verwerpen (p-waarde 0.1987). Met andere woorden: iTunes is willekeurig genoeg.
