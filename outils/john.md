---
description: John the Ripper - Outil de Crack de Mots de Passe
---

# John

<mark style="color:yellow;">Description :</mark>&#x20;

John the Ripper (John) est un puissant outil de crack de mots de passe qui utilise diverses méthodes d'attaque pour récupérer des mots de passe chiffrés dans des fichiers de hachage ou des captures de paquets.

<mark style="color:yellow;">Exemples d'utilisation :</mark>

1. Cracker un fichier de hachage de mots de passe : `john <fichier_de_hachage>`
2. Utiliser une attaque par dictionnaire : `john --wordlist=<fichier_dictionnaire> <fichier_de_hachage>`
3. Utiliser une attaque par force brute (mode incrementation) : `john --incremental <fichier_de_hachage>`

<mark style="color:yellow;">Options Principales :</mark>

* \--wordlist= : Spécifier un fichier contenant un dictionnaire de mots de passe.
* \--rules : Utiliser des règles de transformation pour améliorer les chances de casser le mot de passe.
* \--incremental : Lancer une attaque par force brute en incrémentant les caractères.

<mark style="color:yellow;">Commandes Supplémentaires :</mark>

* `john --show <fichier_de_hachage>` : Afficher les mots de passe crackés.
* `john --list=formats` : Afficher les formats de hachage pris en charge par John.
