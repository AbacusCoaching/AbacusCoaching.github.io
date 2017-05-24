---
layout: post
title:  "Onbetaald parkeren 2"
date:   2017-05-23 21:55:00 +0200
tags: [statistiek,parkeren,boete,poisson]
---
In een vorige blogpost hadden we het al over parkeren zonder te betalen. Toen gingen we ervan uit dat je maar eenmaal beboet kan worden
voor dezelfde overtreding. Maar hoe veranderen de kansen als je meermaals beboet kan worden?


De toevalsvariabele X verandert niet: het is het aantal parkeerwachters die je wagen controleren tijdens je uur onbetaald parkeren.
X is poisson verdeeld met lambda 1 (1 parkeerwachter per uur). De kans op 1 boete is gelijk aan geen boete:


$$
\begin{array}{rcl}
\\P(1 boete)&=&P(X=1) \\\\
&=&\frac{e^{-\lambda}\lambda^x}{x!}\\\\
&=&\frac{e^{-1}1^1}{1!}\\\\
&=&\frac{1}{e}\\\\
&=&0.36787944117
\end{array}
$$


De kans op 2 boetes is gelijkaardig:

$$
\begin{array}{rcl}
\\P(2 boetes)&=&P(X=2) \\\\
&=&\frac{e^{-\lambda}\lambda^x}{x!}\\\\
&=&\frac{e^{-1}1^2}{2!}\\\\
&=&\frac{1}{2*e}\\\\
&=&0.18393972058
\end{array}
$$

En zo verder. Een mooi overzicht met enkele kansen:

|x|	P(X=x)|
|-|-|
|0|	0,367879441|oet
|1|	0,367879441|
|2|	0,183939721|
|3|	0,06131324|
|4|	0,01532831|
|5|	0,003065662|

Maar hoeveel zal je dit nu kosten. Heel gemakkelijk: stel dat een boete 30 euro is. Dan kan je voor de boete een toevalsvariabele B definieren,
en die is gelijk aan 30*X. Dus de kans dat je boete bv 60 euro is, komt overeen met de kans dat je 2 boetes krijgt of

$$
P(B=60)=P(30*X=60)=P(X=2)=0,183939721
$$

Voor de boetes kan je nu ook de kanstabel maken!
