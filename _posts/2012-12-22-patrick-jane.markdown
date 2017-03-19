---
layout: post
title:  "Kan Patrick Jane 20 keer na elkaar kop gooien?"
date:   2012-12-22 15:23:03 +0100
categories: [statistiek,mentalist,hypothese testen]
---
In aflevering 14 van het tweede seizoen van The Mentalist gooit Patrick Jane 20 keer een muntstuk op. Na afloop blijkt hij 20 keer kop gegooid te hebben. Kan dit wel met een **eerlijk** muntstuk?

Een eerlijk muntstuk betekent dat kop evenveel kans heeft als munt, dus de kans op succes is 1/2. Als we X het aantal keer kop noemen bij 20 keer een muntstuk opgooien dan is X binomiaal verdeeld met n=20, p=1/2 en variantie 20\*1/2\*(1-1/2)=5. We berekenen de kans dat je minstens 20 keer kop hebt.

$$
\begin{array}{rcl}
P(X \ge 20)&=&P(X = 20) \\\\
&=&{20 \choose 20}\left( \frac{1}{2} \right)^{20}\\\\
&=&1*0,00000095367431640625
\end{array}
$$

De kans is bijna nul, dus verwerpen we de hypothese dat we met een fair muntstuk te maken hebben.
