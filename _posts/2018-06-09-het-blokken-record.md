---
layout: post
title:  "Het nieuwe blokken record"
date:   2018-06-09 21:19:00 +0200
tags: [statistiek,blokken,record]
---
Het nieuwe [Blokken record](https://www.hln.be/showbizz/tv/-t-is-gebeurd-ewout-vestigt-nieuw-record-in-blokken~ab050b22/) haalde
alle nieuwspagina's! Ewout won elf afleveringen en mag dus beginnen aan de 12e. Maar hoe zit het met
de statistiek achter dit fenomeen? Wat is de kans dat de 12e aflevering verloren wordt?

Hier tellen we eigenlijk het aantal gewonnen afleveringen tot op het moment van het eerste verlies. Natuurlijk
heeft de statistiek hiervoor een kansverdeling, *de geometrische verdeling*.

Laten we aannemen dat de kans om een aflevering van blokken te winnen, 0.4 is. Voor deze vraag heb je
eerst een rij van van 11 winsten gevolgd door een verlies. Als we ervan uit gaat dat de kans op winst voor
elke aflevering onafhankelijk is, dan kom je bij het volgend resultaat uit:

$$
\begin{array}{rcl}
P(\text{11 keer winst gevolgd door verlies})&=&p^{12}(1-p)\\\\
&=&0.4^{12}(1-0.4)\\\\
&=&0.0000100663296
\end{array}
$$

Het is dus inderdaad heel bijzonder om 12 afleveringen na elkaar mee te spelen in blokken.
