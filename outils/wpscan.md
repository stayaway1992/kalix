---
description: WPScan - Outil de Scan de Vulnérabilités WordPress
---

# WPscan

<mark style="color:yellow;">Description :</mark>&#x20;

WPScan est un scanner de sécurité open source spécialement conçu pour les sites WordPress. Il permet de détecter les vulnérabilités, les faiblesses de configuration et les problèmes de sécurité dans les installations WordPress.

<mark style="color:yellow;">Exemples d'utilisation :</mark>

1. Scanner un site WordPress : `wpscan --url http://example.com/`
2. Identifier les utilisateurs : `wpscan --url http://example.com/ --enumerate u`
3. Lister les plugins installés : `wpscan --url http://example.com/ --enumerate p`

<mark style="color:yellow;">Options Principales :</mark>

* \--url : Spécifier l'URL du site WordPress à scanner.
* \--enumerate: Enumérer les utilisateurs (u), les plugins (p) ou les thèmes (t).
* \--passwords : Fournir un fichier contenant des mots de passe pour les attaques de force brute.
* \--random-agent : Utiliser un agent utilisateur aléatoire pour les requêtes.
