---
description: Énumération SSH (Secure Shell) - Cheatsheet
---

# SSH



1. <mark style="color:yellow;">Découverte des hôtes SSH :</mark>
   * `nmap -p 22 <cible>` : Scan du port SSH (port 22) sur un hôte.
2. <mark style="color:yellow;">Identification du système d'exploitation via SSH :</mark>
   * `nmap -p 22 --script ssh-hostkey,ssh2-enum-algos,sshv1 <cible>` : Découvrir le système d'exploitation et les versions de SSH.
3. <mark style="color:yellow;">Connexion SSH en utilisant un nom d'utilisateur et un mot de passe :</mark>
   * `ssh <utilisateur>@<cible>` : Connexion SSH avec un nom d'utilisateur spécifié.
   * `ssh <utilisateur>@<cible> -p <port>` : Connexion SSH sur un port personnalisé.
4. <mark style="color:yellow;">Connexion SSH en utilisant une clé privée :</mark>
   * `ssh -i <chemin_vers_clé_privée> <utilisateur>@<cible>` : Connexion SSH en utilisant une clé privée.
5. <mark style="color:yellow;">Force brute sur SSH :</mark>
   * `hydra -l <utilisateur> -P <liste_mots_de_passe> ssh://<cible>` : Tentative de force brute sur SSH en utilisant une liste de mots de passe.
6. <mark style="color:yellow;">Analyse des utilisateurs via SSH :</mark>
   * `enum4linux -U //<cible>` : Liste des utilisateurs via SMB (parfois utiles pour les connexions SSH).
7. <mark style="color:yellow;">Vérification des vulnérabilités connues :</mark>
   * `ssh -V` : Vérifiez la version actuelle de l'OpenSSH installée.
   * Recherchez les vulnérabilités connues associées à la version spécifique d'OpenSSH.
