---
description: XSSer - Outil d'Exploitation d'Injections XSS
---

# XSSer

<mark style="color:yellow;">Description :</mark>&#x20;

XSSer est un outil open source conçu pour détecter et exploiter les vulnérabilités d'injection de script entre sites (XSS) dans les applications web.

<mark style="color:yellow;">Exemples d'utilisation :</mark>

1. Tester une URL pour les vulnérabilités XSS : `XSSer -u "http://example.com/page.php?id=1"`
2. Utiliser une liste de payloads personnalisés pour les tests : `XSSer -u "http://example.com/search.php?q=test" -p payloads.txt`
3. Utiliser différentes techniques d'injection : `XSSer -u "http://example.com/login.php" -t POST -d "username=admin&password=pass" --auto`

<mark style="color:yellow;">Options Principales :</mark>

* \-u : Spécifier l'URL cible à tester.
* \-p : Fournir un fichier contenant des payloads personnalisés.
* \-t : Spécifier la méthode HTTP à utiliser (GET, POST, etc.).
* \-d : Fournir les données pour une requête HTTP POST.
* \--auto : Activer le mode automatique pour les tests.
