---
description: SQLMap - Outil d'Injection SQL Automatique
---

# SQLMap

<mark style="color:yellow;">Description :</mark>

&#x20;SQLMap est un outil open source qui automatise le processus de détection et d'exploitation des vulnérabilités d'injection SQL dans les applications web.

<mark style="color:yellow;">Exemples d'utilisation :</mark>

1. Tester une URL pour les vulnérabilités d'injection SQL : `sqlmap -u "http://example.com/page.php?id=1"`
2. Tester une URL en utilisant une méthode HTTP POST : `sqlmap -u "http://example.com/login" --data "username=admin&password=pass" --method POST`
3. Enumérer les bases de données : `sqlmap -u "http://example.com/page.php?id=1" --dbs`

<mark style="color:yellow;">Options Principales :</mark>

* \-u : Spécifier l'URL cible à tester.
* \--data : Fournir les données pour une requête HTTP POST.
* \--method \<méthode> : Spécifier la méthode HTTP à utiliser (GET, POST, etc.).
* \--dbs : Enumérer les bases de données disponibles sur le serveur.
