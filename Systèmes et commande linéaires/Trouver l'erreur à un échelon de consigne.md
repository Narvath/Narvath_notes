Pour trouver l'erreur à un échelon de consigne, il faut que l'on connaisse déjà la fonction de transfert _G_ du système $G = G_c G_p$. 

L'erreur est:
$$Consigne - H$$
où $$H = G_{bouclefermee} \times \text{Consigne}$$
et que 
$$G_{boucleFermee}= \frac{K}{1 + K}$$
*En fait, $G_{boucleFermee}$ n'est que la simplification de la fonction de transfert du système lorsqu'on rajoute une boucle de rétroaction négative à la fct de transfert G. C'est G lorsqu'il est mis dans un système!*

Reprenons avec l'exemple suivant en utilisant un échelon unitaire comme entrée *(consigne)* pour tester:
$$G = \frac{18,8}{(1 + \frac{s}{10})(1 + \frac{s}{100})}$$
On aurait ainsi: 
$$\frac{18,8}{1 + 18,8} \times 1$$