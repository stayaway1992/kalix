---
description: DNSenum - Outil d'Enumération DNS
---

# DNSenum

<mark style="color:yellow;">Description :</mark>&#x20;

DNSenum est un outil open source utilisé pour effectuer des énumérations DNS sur un domaine spécifié. Il permet de collecter des informations sur les hôtes, les enregistrements DNS, les sous-domaines et les serveurs de noms associés à la cible.

<mark style="color:yellow;">Exemples d'utilisation :</mark>

1. Effectuer une énumération complète sur un domaine : `dnsenum example.com`
2. Utiliser un fichier contenant une liste de sous-domaines pour l'énumération : `dnsenum -f subdomains.txt example.com`
3. Effectuer une énumération récursive pour trouver des sous-domaines cachés : `dnsenum -r example.com`

<mark style="color:yellow;">Options Principales :</mark>

* \-f : Spécifier un fichier contenant une liste de sous-domaines à énumérer.
* \-r : Effectuer une énumération récursive pour trouver des sous-domaines cachés.
* \-o : Sauvegarder les résultats dans un fichier.
* \-t \<nombre\_de\_threads> : Définir le nombre de threads pour accélérer le scan.

