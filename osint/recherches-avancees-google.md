---
description: Google Dorking - Cheatsheet
---

# Recherches avancees Google

1. <mark style="color:yellow;">Recherche de Pages Sensibles :</mark>
   * Utilisez des requêtes spécifiques pour trouver des pages d'administration, des fichiers de configuration, des bases de données ou des fichiers sensibles : Exemple : intitle:"Index of" /etc/passwd site:example.com intitle:"Login" OR intitle:"Sign in"
2. <mark style="color:yellow;">Découverte de Répertoires :</mark>
   * Recherchez des répertoires cachés ou non indexés : Exemple : site:example.com -inurl:(html|php) intitle:"Index of"
3. <mark style="color:yellow;">Recherche de Fichiers Spécifiques :</mark>
   * Trouvez des fichiers spécifiques tels que des journaux d'accès, des sauvegardes, des fichiers de configuration, etc. : Exemple : site:example.com filetype:log
4. <mark style="color:yellow;">Exploration d'un Domaine Spécifique :</mark>
   * Utilisez la requête "site:" pour rechercher des informations spécifiques sur un domaine donné : Exemple : site:example.com "Confidential" OR "Internal use only"
5. <mark style="color:yellow;">Recherche de Vulnérabilités Connues :</mark>
   * Utilisez des mots-clés spécifiques pour rechercher des vulnérabilités connues : Exemple : "powered by vBulletin" "vBulletin version 3.8.1"
6. <mark style="color:yellow;">Recherche de Données Exposées :</mark>
   * Trouvez des données sensibles ou exposées sur des sites web : Exemple : "password" filetype:txt site:example.com
7. <mark style="color:yellow;">Utilisation de Dorks Préétablis :</mark>
   * Utilisez des dorks préétablis pour cibler des informations spécifiques : Exemple : "inurl:wp-content/uploads"
8. <mark style="color:yellow;">Recherche d'Adresses IP ou de Plages d'IP :</mark>
   * Recherchez des sites web associés à des adresses IP spécifiques : Exemple : "ip:xxx.xxx.xxx.xxx" OR "ip:xxx.xxx.xxx.xxx-xxx"
9. <mark style="color:yellow;">Recherche de Sites Vulnérables :</mark>
   * Utilisez des dorks spécifiques pour trouver des sites vulnérables à des attaques spécifiques : Exemple : "inurl:sql.php?id="
10. <mark style="color:yellow;">Exploitation de Filtres Combinés :</mark>
    * Combiner plusieurs filtres pour affiner votre recherche  : Exemple : site:example.com intext:"Confidential" intitle:"Login"
