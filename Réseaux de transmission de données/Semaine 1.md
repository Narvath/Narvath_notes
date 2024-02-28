## Les 5 couches réseau
 ![[5 couches.png]]

## Délais
### Propagation
- Temps requis pour la propagation du signal dans le médium
- Délais typiquement fix
- distance/vitesse
### Transmission
- Bits d'information du paquet sont transmis sur l'interface réseau
- L'information est transmise à la vitesse de l'interface réseau
- Délai fixe pour une taille fixe de donnée
### Traitement 
- Vérification des erreurs
- Démultiplexage
- Acheminement selon l'adresse destination
- Délai variable
### Mise en file d'attente
- Paquet stocké dans la mémoire de l'interface de sortie
- Temps d'attente dépend de:
	- La quantité de traffic en entrée
	- La vitesse de l'interface de sortie
- Délai variable