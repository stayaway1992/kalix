---
description: Shred - Outil de Suppression Sécurisée de Fichiers
---

# Shred

<mark style="color:yellow;">Description :</mark>&#x20;

Shred est une commande Linux utilisée pour supprimer de manière sécurisée des fichiers en écrivant de manière répétée sur leur contenu. Cela rend plus difficile la récupération des données après la suppression.

<mark style="color:yellow;">Exemples d'utilisation :</mark>

1. Supprimer de manière sécurisée un fichier : `shred -u <nom_du_fichier>`
2. Supprimer de manière sécurisée un répertoire et son contenu : `shred -u -n <nombre_répétitions> -z <nom_du_répertoire>`

<mark style="color:yellow;">Options Principales :</mark>

* \-u : Supprimer le fichier/répertoire après avoir été écrasé.
* \-n \<nombre\_répétitions> : Spécifier le nombre de répétitions d'écriture (3 par défaut).
* \-z : Ajouter une répétition finale avec des zéros pour masquer la suppression.
