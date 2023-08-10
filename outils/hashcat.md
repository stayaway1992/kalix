---
description: Hashcat - Outil de Crack de Hachage
---

# Hashcat

Description :&#x20;

Hashcat est un outil de crack de hachage avancé qui prend en charge une grande variété d'algorithmes de hachage et de méthodes d'attaque pour récupérer des mots de passe chiffrés à partir de fichiers de hachage.

<mark style="color:yellow;">Exemples d'utilisation :</mark>

1. Cracker un fichier de hachage MD5 : `hashcat -a 0 -m 0 <fichier_de_hachage> <fichier_dictionnaire>`
2. Cracker un fichier de hachage SHA256 avec des règles de transformation : `hashcat -a 0 -m 1400 --rules <fichier_de_hachage> <fichier_dictionnaire>`
3. Cracker un fichier de hachage avec une attaque par force brute : `hashcat -a 3 -m 1000 <fichier_de_hachage> ?a?a?a?a?a?a?a?a`

<mark style="color:yellow;">Options Principales :</mark>

* \-a : Spécifier le mode d'attaque (0 pour attaque par dictionnaire, 3 pour attaque par force brute, etc.).
* \-m : Spécifier le type de hachage (0 pour MD5, 1000 pour NTLM, etc.).
* \--rules : Utiliser des règles de transformation pour améliorer les chances de casser le mot de passe.
* ?a : Représente un masque pour une attaque par force brute.

<mark style="color:yellow;">Commandes Supplémentaires :</mark>

* `hashcat --example-hashes` : Afficher des exemples de formats de hachage pris en charge.
* `hashcat --benchmark` : Exécuter un benchmark pour évaluer les performances de votre matériel.
