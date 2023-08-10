---
description: Impacket - Outil pour l'Exploitation Réseau
---

# Impacket

<mark style="color:yellow;">Description :</mark>&#x20;

Impacket est un ensemble d'outils en Python pour l'exploitation de réseaux et de protocoles réseau. Il permet d'interagir avec des services réseau, d'effectuer des attaques et d'exploiter des vulnérabilités dans un environnement réseau.

<mark style="color:yellow;">Exemples d'utilisation :</mark>

1. Lancer une attaque de type SMB Relay : smbrelayx.py
2. Lister les partages SMB d'un hôte distant : smbclient.py -L //\<adresse\_IP>
3. Créer un shell distant en utilisant RCE : psexec.py \<nom\_d'utilisateur>:\<mot\_de\_passe>@\<adresse\_IP>

<mark style="color:yellow;">Options Principales :</mark>

* smbrelayx.py : Attaque de type SMB Relay permettant d'obtenir des informations d'identification d'utilisateurs et d'accéder à des machines cibles via SMB.
* smbclient.py : Client SMB permettant de lister les partages, d'envoyer des fichiers et d'exécuter des commandes sur un serveur SMB distant.
* psexec.py : Exploiter une vulnérabilité de type RCE (Remote Code Execution) pour obtenir un shell distant sur un système cible.

<mark style="color:yellow;">Commandes Supplémentaires :</mark>

* ntlmrelayx.py : Attaque de type NTLM Relay pour exécuter des commandes sur des systèmes distants.
* samrdump.py : Récupérer les informations du registre SAM (Security Account Manager) à partir d'un contrôleur de domaine.
