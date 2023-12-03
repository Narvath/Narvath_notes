---
dg-publish: true
---
Une marge de phase est une mesure de la robustesse d'un système de contrôle en boucle fermée vis-à-vis de la stabilité.

Cette phase importe sur plusieurs points du système soit:
1. **Stabilité**
	1. La marge de phase indique la quantité de phase supplémentaire qu'un système peut tolérer avant de devenir instable (c'est-à-dire avant que la phase atteigne -180 degrés à la fréquence où le gain est de 0 dB)
2. **Robustesse**
	1. Une marge de phase plus grande signifie que le système peut supporter une plus grande variation dans ses paramètres du système ou dans le modèle utilisé pour la conception du contrôleur avant de devenir instable. Cela rend le système plus robuste face aux incertitudes du modèle et aux variations des paramètres.
3. **Réponse Transitoire**
	1. Une marge de phase substantielle influence également la réponse transitoire du système. Une marge de phase plus élevée est généralement associée à une réponse transitoire plus amortie avec moins d'oscillation et un dépassement (overshoot) réduit.
4. **Confort**
	1. Dans beaucoup d'applications pratiques, une marge de phase suffisante contribue non seulement à la stabilité mais aussi au confort d'utilisation et à la performance opérationnelle. Par exemple, dans les systèmes de contrôle de véhicules ou d'avions, une bonne marge de phase assure que le système réagit de manière prévisible et douce aux commandes.

Par exemple, une marge de phase de 30$\degree$ donnerait une phase de :
-180 $\degree$ + 30$\degree$ = -150$\degree$. Lorsqu'on optimise le K d'une fonction de transfert à ce déphasage, il devient le point critique de stabilité du système. Il aurait toutefois une marge de stabilité de 30$\degree$ avant d'atteindre -180$\degree$ et de devenir instable.