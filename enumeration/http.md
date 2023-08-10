---
description: Énumération HTTP - Cheatsheet
---

# HTTP



1. <mark style="color:yellow;">Découverte des hôtes HTTP  :</mark>

* nmap -p 80,443 `<cible>` : Scan des ports HTTP (80 pour HTTP, 443 pour HTTPS).

1. <mark style="color:yellow;">Identification du système d'exploitation via HTTP :</mark>
   * `nmap -p 80,443 --script http-enum <cible>` : Découvrir le système d'exploitation et les versions de serveur HTTP.
2. <mark style="color:yellow;">Analyse du serveur web :</mark>
   * `curl -I <URL>` : Obtenir les en-têtes HTTP du serveur web.
   * `curl -A "<user_agent>" <URL>` : Envoyer un en-tête personnalisé avec une requête HTTP.
3. <mark style="color:yellow;">Liste des répertoires et fichiers :</mark>
   * `gobuster dir -u <URL> -w <wordlist>` : Enumérer les répertoires et les fichiers avec gobuster et une liste de mots.
   * `dirb <URL><wordlist>`: Enumérer les répertoires et les fichiers avec dirb et une liste de mots.
4. <mark style="color:yellow;">Recherche de vulnérabilités :</mark>
   * Nikto : Utiliser Nikto pour identifier les vulnérabilités connues sur le serveur web.
   * `nmap --script http-vuln* <cible>` : Utiliser Nmap pour rechercher des vulnérabilités spécifiques liées à HTTP.
5. <mark style="color:yellow;">Fuzzing de paramètres :</mark>
   * Burp Suite : Utiliser Burp Suite pour le fuzzing de paramètres et la découverte de vulnérabilités d'injection (SQL, XSS, etc.).
   * wfuzz : Utiliser wfuzz pour le fuzzing des paramètres avec des listes de valeurs potentielles.
6. <mark style="color:yellow;">Capture de requêtes et réponses :</mark>
   * Burp Suite : Capturer les requêtes HTTP/HTTPS pour les analyser et les modifier.
   * Wireshark : Capturer et analyser le trafic HTTP brut.
7. <mark style="color:yellow;">Analyse des cookies :</mark>
   * EditThisCookie (extension de navigateur) : Examiner, modifier et tester les cookies du site web.
