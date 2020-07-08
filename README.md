# geolocalisation-LoRa
Système de géolocalisation utilisant la technologie LoRa, comprenant des trackers, des relais et un gateway.
# 1. Partie Tracker

Cette partie comporte un tracker STM (STEVAL-STRKT01 ) qui permet de récupérer les coordonnées GPS ainsi que les valeurs d'un accéléromètre.
![alt tag](https://github.com/diegopanepo/geolocalisation-LoRa/blob/master/Images/tracker.jpg)
# 2. Partie Relai

Cette partie comporte une carte LoRa UCA qui permet de récupérer des données d'un émetteur LoRa et de les retransmettre ce qui permet de recevoir les données du tracker de plus loin.
![alt tag](https://github.com/diegopanepo/geolocalisation-LoRa/blob/master/Images/relay.jpg)
# 2. Partie Gateway

Cette partie comporte une carte LoRa UCA qui permet de récupérer des données d'un émetteur LoRa et une Raspberry Pi 4.
![alt tag](https://github.com/diegopanepo/geolocalisation-LoRa/blob/master/Images/gateway.jpg)
La carte LoRa est connecté par le port USB à la Raspberry. Celle-ci en utlisant Node-RED peut récupérer les données reçu.
En connectant la Raspberry à Internet, nous pouvons utiliser Node-RED.
Grâce à Node-RED, nous pouvons ensuite afficher ces données sur un tableau de bord.
Celui-ci comporte pour les tests, les données du tracker (données GPS, accéléromètre, etc... ).
A partir des données GPS, nous affichons sur notre tableau de bord à partir de Google Maps leurs positions.
