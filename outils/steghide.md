---
description: Steghide - Outil de Dissimulation de Données dans des Médias
---

# Steghide

<mark style="color:yellow;">**Description :**</mark>&#x20;

Steghide est un outil open source permettant de cacher des données confidentielles à l'intérieur de fichiers média, tels que des images et des fichiers audio.

<mark style="color:yellow;">**Exemples d'utilisation :**</mark>

1. Cacher des données dans une image : `steghide embed -cf  -ef <fichier_caché>`
2. Extraire des données cachées d'une image : `steghide extract -sf`&#x20;

<mark style="color:yellow;">**Options Principales :**</mark>

* embed : Cacher des données dans un fichier média.
* extract : Extraire des données cachées d'un fichier média.
* \-cf  : Spécifier le fichier média de couverture (image).
* \-ef \<fichier\_caché> : Spécifier le fichier à cacher.
* \-sf  : Spécifier le fichier média à partir duquel extraire les données.
