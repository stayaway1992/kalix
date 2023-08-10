---
description: Énumération FTP (File Transfer Protocol) - Cheatsheet
---

# FTP



1. <mark style="color:yellow;">Découverte des hôtes FTP :</mark>
   * `nmap -p 21 <cible>` : Scan du port FTP (port 21) sur un hôte.
2. <mark style="color:yellow;">Identification du système d'exploitation via FTP :</mark>
   * `nmap -p 21 --script ftp-anon,ftp-bounce,ftp-libopie,ftp-proftpd,ftp-vsftpd-backdoor <cible>` : Découvrir le système d'exploitation et les vulnérabilités liées à FTP.
3. <mark style="color:yellow;">Connexion anonyme :</mark>
   * `ftp <cible>` : Connexion anonyme au serveur FTP.
   * Nom d'utilisateur : anonymous
   * Mot de passe : `<adresse_email>` ou simplement un espace (selon la configuration du serveur).
4. <mark style="color:yellow;">Connexion avec des identifiants :</mark>
   * `ftp <cible>` : Connexion au serveur FTP en utilisant un nom d'utilisateur et un mot de passe.
5. <mark style="color:yellow;">Listage des répertoires :</mark>
   * `ls` : Afficher la liste des fichiers et répertoires du répertoire actuel.
   * `ls <répertoire>` : Afficher la liste des fichiers et répertoires d'un répertoire spécifique.
6. <mark style="color:yellow;">Récupération de fichiers :</mark>
   * `get <fichier>` : Télécharger un fichier depuis le serveur FTP vers le répertoire local.
   * `mget *` : Télécharger tous les fichiers du répertoire actuel vers le répertoire local.
7. <mark style="color:yellow;">Changement de répertoire :</mark>
   * `cd <répertoire>` : Aller dans le répertoire spécifié sur le serveur FTP.
8. <mark style="color:yellow;">Transfert de fichiers vers le serveur :</mark>
   * `put <fichier>` : Envoyer un fichier depuis le répertoire local vers le serveur FTP.
   * `mput *` : Envoyer tous les fichiers du répertoire local vers le serveur FTP.
9. <mark style="color:yellow;">Suppression de fichiers :</mark>
   * `delete <fichier>` : Supprimer un fichier du serveur FTP.
10. <mark style="color:yellow;">Création de répertoire :</mark>
    * `mkdir <répertoire>` : Créer un nouveau répertoire sur le serveur FTP.
11. <mark style="color:yellow;">Suppression de répertoire :</mark>
    * `rmdir <répertoire>` : Supprimer un répertoire vide du serveur FTP.
