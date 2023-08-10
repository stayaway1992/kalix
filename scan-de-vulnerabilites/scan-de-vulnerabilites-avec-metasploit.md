---
description: Scan de Vulnérabilités avec Metasploit - Cheatsheet
---

# Scan de vulnerabilites avec Metasploit

<mark style="color:red;">**Disclaimer : je ne peux que vous conseillez de regarder une vidéo sur comment utiliser Metasploit une cheatsheet étant bien trop modeste pour le comprendre et apprendre à l'utiliser**</mark>

1. <mark style="color:yellow;">Lancement de Metasploit :</mark>
   * Ouvrez un terminal et lancez `msfconsole` pour démarrer l'interface de Metasploit.
2. <mark style="color:yellow;">Mise à jour des modules :</mark>
   * Mettez à jour les modules de Metasploit en utilisant la commande `msfupdate` dans le terminal.
3. <mark style="color:yellow;">Recherche de modules :</mark>
   * Utilisez la commande `search <nom_module>` pour rechercher des modules de scan de vulnérabilités.
4. <mark style="color:yellow;">Sélection d'un module de scan :</mark>
   * Utilisez la commande `use <nom_module>` pour charger un module de scan spécifique.
5. <mark style="color:yellow;">Affichage des options du module :</mark>
   * Utilisez la commande `show options` pour afficher les options du module de scan.
6. <mark style="color:yellow;">Configuration des options du module :</mark>
   * Utilisez la commande `set <option> <valeur` pour configurer les options du module (par exemple : set RHOSTS 192.168.1.10).
7. <mark style="color:yellow;">Exécution du scan :</mark>
   * Utilisez la commande `run` pour lancer le scan de vulnérabilités.
8. <mark style="color:yellow;">Analyse des résultats du scan :</mark>
   * Après l'exécution du scan, utilisez les commandes `vulns` ou `hosts` pour afficher les vulnérabilités identifiées ou les hôtes vulnérables.
9. <mark style="color:yellow;">Utilisation d'un scan plus spécifique :</mark>
   * Certaines modules de scan prennent en charge des options spécifiques pour des vulnérabilités ou des services particuliers.
10. <mark style="color:yellow;">Exploitation des vulnérabilités identifiées :</mark>
    * Une fois les vulnérabilités identifiées, vous pouvez utiliser Metasploit pour tenter des exploits contre les hôtes vulnérables.
