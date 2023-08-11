---
description: GPG - GNU Privacy Guard - Cheat Sheet
---

# GPG

<mark style="color:yellow;">GPG Introduction :</mark>&#x20;

GPG (GNU Privacy Guard) est un outil de chiffrement et de signature numérique qui offre une sécurité renforcée pour la communication et le stockage de données sensibles.

1. Générer une nouvelle paire de clés : `gpg --gen-key`
2. Afficher les clés disponibles : `gpg --list-keys`
3. Chiffrer un fichier avec la clé publique d'un destinataire : `gpg -e -r <email_destinataire>`
4. Décrypter un fichier chiffré : `gpg -d <fichier_chiffré>`
5. Signer un fichier avec votre clé privée : `gpg --sign`
6. Vérifier la signature d'un fichier : `gpg --verify <fichier.sig>`
7. Exporter une clé publique : `gpg --armor --export > pubkey.asc`
8. Importer une clé publique : `gpg --import pubkey.asc`
9. Changer le niveau de confiance d'une clé : `gpg --edit-key`
10. Révoquer une clé : `gpg --gen-revoke > revoke.asc`

<mark style="color:yellow;">Options Principales :</mark>

* \--gen-key : Générer une nouvelle paire de clés.
* \--list-keys : Afficher les clés disponibles.
* \-e : Chiffrer un fichier.
* \-r : Spécifier le destinataire lors du chiffrement.
* \-d : Décrypter un fichier.
* \--sign : Signer un fichier.
* \--verify : Vérifier la signature d'un fichier.
* \--armor : Exporter au format ASCII (lisible).
* \--export : Exporter une clé publique.
* \--import : Importer une clé publique.
