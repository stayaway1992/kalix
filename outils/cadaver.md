---
description: Cadaver - Client WebDAV en Ligne de Commande
---

# Cadaver

<mark style="color:yellow;">Description :</mark>&#x20;

Cadaver est un client WebDAV en ligne de commande qui permet d'interagir avec des serveurs WebDAV pour le transfert de fichiers et la gestion de contenu distant.

<mark style="color:yellow;">Exemples d'utilisation :</mark>

1. Se connecter à un serveur WebDAV distant : `cadaver http://example.com/dav/`
2. Afficher la liste des fichiers et répertoires : `cadaver> ls`
3. Télécharger un fichier depuis le serveur WebDAV : `cadaver> get fichier.txt`
4. Envoyer un fichier vers le serveur WebDAV : `cadaver> put fichier.txt`

<mark style="color:yellow;">Options Principales :</mark>

* `ls`: Afficher la liste des fichiers et répertoires sur le serveur distant.
* `get`: Télécharger un fichier depuis le serveur WebDAV vers le répertoire local.
* `put`: Envoyer un fichier depuis le répertoire local vers le serveur WebDAV.

<mark style="color:yellow;">Commandes Supplémentaires :</mark>

* `cd <répertoire>` : Changer de répertoire distant.
* `mkdir <répertoire>` : Créer un répertoire sur le serveur WebDAV.
* `delete <fichier/répertoire>` : Supprimer un fichier ou un répertoire sur le serveur distant.
