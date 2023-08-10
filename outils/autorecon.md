---
description: Autorecon - Outil d'Automatisation pour la Reconnaissance de Systèmes
---

# Autorecon

<mark style="color:yellow;">Description :</mark>&#x20;

Autorecon est un outil d'automatisation écrit en Python conçu pour faciliter et accélérer la phase de reconnaissance dans les tests d'intrusion. Il automatise les tâches de collecte d'informations sur les cibles en utilisant diverses techniques et outils.

<mark style="color:yellow;">Exemples d'utilisation :</mark>

1. Lancer une analyse rapide de reconnaissance sur une cible : `autorecon <adresse_IP>`
2. Exécuter une analyse approfondie avec un dictionnaire personnalisé : `autorecon -c <chemin_dictionnaire> <adresse_IP>`
3. Lancer une analyse de port spécifique : `autorecon -p <numéro_port> <adresse_IP>`

<mark style="color:yellow;">Options Principales :</mark>

* \-c \<chemin\_dictionnaire> : Spécifier un dictionnaire personnalisé pour l'analyse de domaine.
* \-p \<numéro\_port> : Exécuter l'analyse sur un port spécifique.

<mark style="color:yellow;">Fonctionnalités Clés :</mark>

* Recherche DNS : Collecter des informations sur les enregistrements DNS (sous-domaines, hôtes, adresses IP, etc.).
* Scan de Ports : Détecter les ports ouverts et les services en cours d'exécution.
* Capture de Bannière : Collecter les bannières des services pour identifier les versions logicielles.
* Analyse Web : Enumérer les répertoires, trouver des fichiers intéressants, etc.
* Recherche d'Informations : Collecter des informations publiques sur les domaines et les adresses IP.
