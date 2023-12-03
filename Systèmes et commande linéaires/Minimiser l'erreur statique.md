---
quickshare-date: 2023-12-02 20:21:25
quickshare-url: "https://noteshare.space/note/clposr0vd207201mw7f38mvvj#OiBeas/eavU49TU3THCUrq9FTijoAYmpQgC0f4NT/gE"
---
Pour minimiser l'[[Erreur Statique]], vous souhaitez que le gain (K) à basse fréquence (approchant de ω=0) soit élevé, car cela indique une forte réaction aux erreurs constantes dans le système. 

En termes de fonctions de transfert, cela signifie que le terme intégral (I) doit être augmenté.

Voici un exemple ou on souhaite trouver un K minimisant l'erreur statique du système suivant:
$$G_{p} = \frac{10}{(1 + \frac{s}{10})(1 + \frac{s}{100})}$$
*Sachant qu'on veux garder une [[Marge de phase]] de 45$\degree$ :* 

Voici les étapes de résolution :
1. Déterminer la phase ($\theta \text{rad}$) a laquelle on veux avoir un gain de 0dB et un module de 1
   Cela est généralement -180$\degree$ + Marge de phase (ici 45$\degree$)
$$
   \theta \text{rad} = (-180 + 45) \times \frac{\pi}{180}
$$
2. On peux par la suite calculer la fréquence $\omega_{0}$ à laquelle on obtient ce déphasage en se servant de cette formule:$$
	\theta \text{rad} = -arctan(\tau \times \omega_{0}) - \text{... des autres poles}
$$ ce qui donne:
$$
\frac{-3}{4\pi} = -arctan(\frac{\omega_{0}}{10}) -arctan(\frac{\omega_{0}}{100})
$$
$$
\omega_{0} = 120\text{rad/s}
$$
3. Comme on sait qu'à cette fréquence on a un module de 1, on n'a qu'a égaler le module de la fonction de transfert (en remplaçant s par $\omega_{0}$) à 1 et à isoler le _K_ de la fonction.
$$
|G(j120)| =\frac{10K}{\sqrt{1 + \left(\frac{120}{10}\right)^2} \cdot \sqrt{1 + \left(\frac{120}{100}\right)^2}} = 1
$$
$$K \approx 1,88$$

