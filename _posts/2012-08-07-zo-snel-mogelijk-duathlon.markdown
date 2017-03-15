---
layout: post
title:  "Hoe leg je zo snel mogelijk een duathlon af?"
date:   2012-08-07 15:14:31 +0200
categories: wiskunde afgeleide optimaliseren
---
De atleet loopt een wedstrijd rond een vijver met straal 20 meter.  Hij moet zo snel mogelijk naar de finish F die zich recht aan de overkant bevindt van de start S. Hij loopt langs de rand van de vijver, en vanaf een willekeurig moment duikt hij in het water en zwemt in een rechte lijn naar de finish. Waar springt hij het best in het water als hij dubbel zo snel loopt als zwemt?

Het duikpunt D ligt dus op de cirkel die de vijver voorstelt. Het midden van de vijver wordt O genoemd. Veronderstel even dat het lijnstuk DO een hoek theta vormt met de horizontale. De cirkelboog SD meet dan

$$|SD|=\theta * 20$$

De lengte van het lijnstuk duikpunt-finish DF kan je berekenen met eenvoudige driehoeksmeetkunde **tip: maak een schets!**

$$|DF|=40\sin(\frac{\pi-\theta}{2})$$

De totale tijd om de volledige afstand af te leggen is de looptijd + de zwemtijd. Als de zwemsnelheid k m/s is, dan is de loopsnelheid 2k m/s, dus de functie voor de totale tijd wordt:

$$
\begin{array}{rcl}
tijd(\theta)&=&\frac{|SD|}{2k}+\frac{|DF|}{k}\\\\
&=&\frac{\theta * 20}{2k}+\frac{40}{k}\sin(\frac{\pi-\theta}{2})
\end{array}
$$

Het moeilijk werk is achter de rug. Nu hoeft enkel nog de functie afgeleid worden naar theta, het nulpunt zoeken en controleren of deze oplossing inderdaad een minumum is. Je zal ook zien dan de ongekende snelheid k zal wegvallen!
