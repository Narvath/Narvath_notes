---
quickshare-date: 2023-12-03 13:36:55
quickshare-url: "https://noteshare.space/note/clpptqqu5360001mwync5a3nj#CzjQ2661WdajuGVQiQioqaF3gQUfFmGaIA/cjV2OO/A"
---
Pour trouver l'erreur à un échelon de consigne, il faut que l'on connaisse déjà la fonction de transfert _G_ du système $G = G_c G_p$. 

Ce que l'on cherche est l'erreur :
$$\epsilon = \text{Consigne} - (\text{gain statique de H} \times Consigne)$$
où
$$\text{gain statique de H}= \frac{K}{1 + K}$$
Reprenons avec l'exemple suivant en utilisant un échelon unitaire comme entrée *(consigne)* pour tester:
$$G = \frac{18,8}{(1 + \frac{s}{10})(1 + \frac{s}{100})}$$
On aurait ainsi: 
$$1 - (\frac{18,8}{1 + 18,8} \times 1) = 0,05$$

TLDR: 
1. On rajoute une boule de rétroaction à G pour en faire un système ($G_{boucleFermee}$) et on le multiplie par l'entée du système.
2. On prends le Feedback du système (H) et on le multiplie par l'entée du système.
3. On soustraie les deux et cela donne l'erreur à la consigne