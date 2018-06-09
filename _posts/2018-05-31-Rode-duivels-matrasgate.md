---
layout: post
title:  "Matrasgate - op hoeveel manieren laat je 5 spelers thuis?"
date:   2018-05-31 22:52:00 +0200
tags: [statistiek,wk,rode duivels]
---
[Matrasgate](https://www.hln.be/sport/voetbal/buitenlands-voetbal/wk-voetbal/matrasgate-deze-vijf-rode-duivels-gaan-niet-naar-wk-als-we-matrassen-mogen-geloven~aa5b9870/) is het woord van de week. Het verwijst naar de matrasfabrikant die
elke matras voor het nationale elftal vernoemt naar een Rode duivel. Aanhangers
van complottheorieën concludeerden hiermee dat de selectie voor het WK
in Rusland definitief was. Maar is dat wel zo? *Statistics to the rescue!*

Tot nu toe was er een voorlopige selectie van 28 spelers. Die moest nog verder gereduceerd worden tot 23. Op fotos konden de namen op de matrassen gelezen worden en wie ontbrak op het lijstje?

* Leander Dendoncker
* Matz Sels
* Jordan Lukaku
* Adnan Januzaj
* Christian ­Kabasele

Maar wat is nu de kans dat als maandag de selectie bekend gemaakt wordt door de bondscoach, deze 5 effectief niet spelen?

Dit is gewoon een toepassing van 5 personen kiezen uit een groep van 28 waarbij de volgorde van selectie onbelangrijk is. Dan kom je automatisch bij binomiaal getallen uit.

$$
\begin{array}{rcl}
\binom{28}{5}&=&\frac{28!}{5!(28-5)!}\\\\
&=&98280
\end{array}
$$

Je kan dus op 98280 manieren 5 personen kiezen. Dus de kans dat net deze 5 niet opgenomen worden in de select is 1/98280, zeer klein dus.

**Update** Collega's Morgan en Jeffrey vertelden mij dat 16 spelers zo goed als zeker zijn van de selectie. Dus dan verandert dit probleem in 5 personen kiezen uit 12:

$$
\begin{array}{rcl}
\binom{12}{5}&=&\frac{12!}{5!(12-5)!}\\\\
&=&792
\end{array}
$$

De kans wordt dan 1/792, veel groter dus maar nog altijd kleiner dan 0.1 procent.
