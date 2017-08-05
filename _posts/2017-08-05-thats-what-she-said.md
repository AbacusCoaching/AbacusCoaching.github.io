---
layout: post
title:  "That's what she said"
date:   2017-08-05 23:05:00 +0200
tags: [statistiek,the office US,poisson]
---
In de Amerikaanse remake van The Office gebruikt regional manager Michael Scott te pas en te onpas de catchphrase 'That's what she said'.

De reeks liep gedurende 9 seizoen, elk 23 afleveringen van 25 minuten. Tijdens deze 9 seizoenen werd die beruchte zin [48 keer](http://theoffice.wikia.com/wiki/List_of_the_times_somebody_says_%22That%27s_what_she_said%22) gezegd. Wat is de kans dat die 1 keer in een aflevering voorkomt?

Dit is -opnieuw- een voorbeeld van een poisson proces, deze keer met een gemiddelde van 48 keer voor alle afleveringen. In een vorige post werd duidelijk dat het gemiddeld proportioneel de tijdsduur is. Het gemiddelde voor 1 aflevering is dus 48/(9*23) = 0,2318840579712

$$
\begin{array}{rcl}
\\P(1 keer)&=&P(X=1) \\\\
&=&\frac{e^{-\lambda}\lambda^x}{x!}\\\\
&=&\frac{e^{-0.2318840579712}0.2318840579712^1}{1!}\\\\
&=&\frac{0.2318840579712}{e^0.2318840579712}\\\\
&=&0.18389288450305
\end{array}
$$

De kans op 1 keer de catchphrase horen tijdens een willekeurige aflevering is 0.18 of bijna 1 aflevering op 5.
