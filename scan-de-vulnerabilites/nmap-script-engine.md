---
description: Nmap Script Engine (NSE) - Cheatsheet
---

# Nmap Script Engine

1. <mark style="color:yellow;">Exécution de scripts NSE :</mark>
   * `nmap -p <ports> --script <script> <cible>` : Exécuter un script NSE spécifique sur les ports spécifiés.
   * `nmap -p <ports> --script "not <script>" <cible>` : Exclure un script NSE spécifique.
2. <mark style="color:yellow;">Sélection de scripts NSE basée sur les catégories :</mark>
   * `nmap --script <catégorie> <cible>` : Exécuter tous les scripts NSE de la catégorie spécifiée.
   * `nmap --script "default" <cible>` : Exécuter les scripts NSE par défaut (sélectionnés par Nmap).
3. <mark style="color:yellow;">Découverte de vulnérabilités avec NSE :</mark>
   * `nmap --script vuln <cible>` : Exécuter des scripts NSE pour la découverte de vulnérabilités.
   * `nmap --script "vuln and safe" <cible>` : Exécuter uniquement des scripts de découverte de vulnérabilités sans causer de dommages.
4. <mark style="color:yellow;">Scripts de récupération d'informations :</mark>
   * `nmap --script discovery <cible>` : Exécuter des scripts de récupération d'informations sur la cible.
   * `nmap --script smb-os-discovery <cible>` : Découvrir les systèmes d'exploitation Windows via SMB.
5. <mark style="color:yellow;">Scripts de sécurité :</mark>
   * `nmap --script "http* and not brute" <cible>` : Exécuter des scripts de sécurité pour les services HTTP sans effectuer de bruteforce.
6. <mark style="color:yellow;">Personnalisation des scripts NSE :</mark>
   * Copiez les scripts personnalisés dans le répertoire "nmap/scripts" pour qu'ils soient accessibles par Nmap.
   * Utilisez des options de scripts pour les adapter à des cas d'utilisation spécifiques.
7. <mark style="color:yellow;">Mise à jour des scripts NSE :</mark>
   * `nmap --script-updatedb` : Mettre à jour la base de données des scripts NSE.
