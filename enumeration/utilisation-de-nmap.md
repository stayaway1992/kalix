---
description: Apprendre à utiliser Nmap - cheatsheet
---

# Utilisation de nmap



1. <mark style="color:yellow;">Découverte des hôtes :</mark>
   * `nmap <cible>` : Scan de base sur une adresse IP ou un nom d'hôte.
   * `nmap <plage_IP>` : Scan sur une plage d'adresses IP.
   * `nmap -iL <fichier>` : Scan sur une liste d'adresses IP/hosts depuis un fichier.
2. <mark style="color:yellow;">Scans de base :</mark>
   * `nmap -sP <cible>` : Découverte des hôtes vivants (Ping scan).
   * `nmap -sS <cible>` : Scan TCP SYN (Scan de ports).
   * `nmap -sU <cible>` : Scan UDP (Scan de ports).
3. <mark style="color:yellow;">Détection de version de service :</mark>
   * `nmap -sV <cible>` : Détecte les versions des services en cours d'exécution.
4. <mark style="color:yellow;">Scan de tous les ports :</mark>
   * `nmap -p- <cible>` : Scan de tous les ports (1-65535).
5. <mark style="color:yellow;">Scans spécifiques de port :</mark>
   * `nmap -p <ports> <cible>` : Scan des ports spécifiés (ex. 80,443,8080).
   * `nmap -F <cible>` : Scan rapide des 100 ports les plus courants.
6. <mark style="color:yellow;">Scan rapide :</mark>
   * `nmap -T4 <cible>` : Scan rapide en mode agressif.
7. <mark style="color:yellow;">Détection d'OS :</mark>
   * `nmap -O <cible>` : Détection du système d'exploitation.
8. <mark style="color:yellow;">Scripts NSE (Nmap Scripting Engine) :</mark>
   * `nmap -sC <cible>` : Exécute les scripts de base.
   * `nmap --script <script><cible>` : Exécute un script spécifique.
9. <mark style="color:yellow;">Scan en mode silencieux :</mark>
   * `nmap -sS -T5 -Pn --open <cible>` : Scan rapide, sans ping, en affichant uniquement les hôtes ouverts.
10. <mark style="color:yellow;">Génération de rapports :</mark>
    * `nmap -oN <fichier> <cible>` : Enregistre la sortie dans un fichier texte.
    * `nmap -oX <fichier> <cible>` : Enregistre la sortie dans un fichier XML.
