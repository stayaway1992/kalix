---
description: TheHarvester - Outil de Collecte d'Informations
---

# theHarvester

<mark style="color:yellow;">Description :</mark>&#x20;

theHarvester est un outil de collecte d'informations open source utilisé pour extraire des informations sensibles telles que les adresses e-mail, les noms de domaine, les sous-domaines et les emplacements IP associés à une cible spécifique à partir de sources publiques.

<mark style="color:yellow;">Exemples d'utilisation :</mark>

1. Rechercher des adresses e-mail associées à un domaine : `theHarvester -d example.com -b google`
2. Extraire des sous-domaines : `theHarvester -d example.com -b bing`
3. Collecter des informations sur un domaine à partir de toutes les sources disponibles : `theHarvester -d example.com -b all`

<mark style="color:yellow;">Options Principales :</mark>

* \-d : Spécifier le domaine cible.
* \-b \<moteur\_de\_recherche> : Sélectionner le moteur de recherche à utiliser (google, bing, yahoo, etc.).
* \-l \<nombre\_de\_résultats> : Limiter le nombre de résultats retournés par le moteur de recherche.
* \-f : Enregistrer les résultats dans un fichier.
