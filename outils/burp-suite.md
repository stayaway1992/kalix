---
description: Burp Suite - Outil d'Analyse de Sécurité Web
---

# Burp Suite

<mark style="color:red;">Disclaimer : je ne peux que vous conseillez de regarder une vidéo sur comment utiliser Burp,       une cheatsheet étant bien trop modeste pour le comprendre et apprendre à l'utiliser</mark>



_Pour faire une attaque login avec_ [_Burp_](../pentest-dapplication-web/login-avec-burp.md)

<mark style="color:yellow;">Description :</mark>&#x20;

Burp Suite est une suite d'outils complète conçue pour l'analyse de sécurité des applications web. Elle comprend un proxy HTTP, un analyseur de site, un scanner de vulnérabilités, un testeur d'intrusion et d'autres fonctionnalités pour aider les professionnels de la sécurité à identifier et à corriger les vulnérabilités des applications web.

<mark style="color:yellow;">Exemples d'utilisation :</mark>

1. Configuration du navigateur pour utiliser le proxy Burp :
   * Configurer le navigateur pour utiliser le proxy Burp sur le port 8080.
2. Découverte des vulnérabilités :
   * Utiliser l'outil "Spider" pour parcourir le site et découvrir les pages et les fonctionnalités.
   * Utiliser le "Scanner" pour identifier les vulnérabilités telles que les injections SQL, les XSS, etc.
3. Interception des requêtes et des réponses :
   * Utiliser le proxy Burp pour intercepter et modifier les requêtes et réponses entre le navigateur et le serveur web.
4. Test d'intrusion avec Burp Intruder :
   * Utiliser l'outil "Intruder" pour tester l'injection de paramètres, l'authentification, etc.
5. Recherche de mots de passe avec Burp Decoder :
   * Utiliser l'outil "Decoder" pour encoder/décoder des chaînes, y compris la recherche de mots de passe en base64.

<mark style="color:yellow;">Options Principales :</mark>

* Proxy : Intercepter et modifier le trafic HTTP entre le navigateur et le serveur.
* Spider : Découvrir et cartographier les pages d'un site.
* Scanner : Identifier les vulnérabilités web.
* Intruder : Tester l'injection de paramètres.
* Decoder : Encoder/décoder des chaînes, y compris la recherche de mots de passe en base64.
