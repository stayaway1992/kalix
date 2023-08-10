---
description: Banner Grabbing avec Netcat (nc) - Cheatsheet
---

# Banner grabbing avec netcat



1. <mark style="color:yellow;">Récupération de bannière sur un port spécifique :</mark>

* `nc -v <hôte> <port>` : Connexion au port spécifié sur l'hôte distant et affichage de la bannière (si disponible).

2. <mark style="color:yellow;">Récupération de bannières pour plusieurs ports :</mark>

* `for port in $(seq <port_debut> <port_fin>); do nc -v -n -z -w1 <hôte> $port; done` : Vérification de la bannière sur une plage de ports.
