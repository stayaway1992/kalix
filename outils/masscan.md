---
description: Cheatsheet Masscan
---

# Masscan

<mark style="color:yellow;">Description :</mark>&#x20;

Masscan est un scanner de ports rapide et léger, conçu pour effectuer des analyses rapides sur de larges plages d'adresses IP.

<mark style="color:yellow;">Exemples d'utilisation :</mark>

1. Analyser un seul hôte : `masscan -p 1-65535 <adresse_IP>`
2. Analyser un sous-réseau : `masscan -p 80,443 <adresse_IP_Range>`
3. Spécifier la vitesse du scan (packets par seconde) : `masscan -p 22 <adresse_IP> --rate 10000`
4. Sauvegarder les résultats dans un fichier : `masscan -p 3389 <adresse_IP> -oG resultat.txt`

<mark style="color:yellow;">Options Principales :</mark>

* \-p : Spécifier les ports à scanner (exemple: -p 80,443,3389).
* \--rate \<packets\_par\_seconde> : Définir la vitesse du scan.
* \-oG : Sauvegarder les résultats dans un fichier au format greppable.
* \--exclude \<adresse\_IP> : Exclure une adresse IP du scan.
