---
description: Binwalk - Outil d'Analyse de Fichiers et d'Images
---

# Binwalk

<mark style="color:yellow;">Description :</mark>&#x20;

Binwalk est un outil open source conçu pour l'analyse et l'extraction d'informations à partir de fichiers et d'images, tels que les images système, les firmwares et les archives compressées.

<mark style="color:yellow;">Exemples d'utilisation :</mark>

1. Analyser un fichier pour les signatures de fichiers connus : `binwalk`
2. Extraire les fichiers intégrés dans une image : `binwalk -e`
3. Recherche récursive d'images dans un répertoire : `binwalk -r <répertoire>`

<mark style="color:yellow;">Options Principales :</mark>

* \-e : Extraire les fichiers intégrés dans l'image.
* \-r : Rechercher récursivement dans un répertoire.
* \-D : Désactiver la signature automatique.
* \-M : Afficher les résultats au format Machine.
* \-l : Liste des signatures de fichiers connus.
