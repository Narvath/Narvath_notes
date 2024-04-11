# Les services de la couche transport
- multiplexage et démultiplexage
- transmission fiable des données
- contrôle de flux
- contrôle de congestion

UDP : sans connexion
	Identifié par l'adresse IP <mark style="background: #FFB86CA6;">destination</mark> et numéro de port <mark style="background: #FFB86CA6;">destination</mark>
TCP : avec connexion
	Identifié par l'adresse IP <mark style="background: #BBFABBA6;">source</mark> et <mark style="background: #FFB86CA6;">destination</mark> et numéro de port <mark style="background: #BBFABBA6;">source</mark> et <mark style="background: #FFB86CA6;">destination</mark>

La couche transport fait la communication logique entre les processus (applications) sur les appareils.

## Multi/démultiplexage
doit identifier vers quelle application acheminer le message. 
	Correspond au socket réseau utilisé par l'application
### Socket
Un socket réseau est une porte entre l'application et le réseau.

