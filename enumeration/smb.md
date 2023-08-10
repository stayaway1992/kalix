---
description: Énumération SMB (Server Message Block) - Cheatsheet
---

# SMB



1. <mark style="color:yellow;">Découverte des hôtes SMB :</mark>
   * `nmap -p 139,445 <cible>` : Scan des ports SMB (139 pour NetBIOS, 445 pour SMB).
2. <mark style="color:yellow;">Identification du système d'exploitation via SMB :</mark>
   * `nmap -p 445 --script smb-os-discovery <cible>` : Découvrir le système d'exploitation des hôtes SMB.
3. <mark style="color:yellow;">Liste des partages SMB :</mark>
   * `smbclient -L //<cible>` : Liste des partages SMB disponibles.
   * `nmap -p 445 --script smb-enum-shares <cible>` : Découvrir les partages SMB.
4. <mark style="color:yellow;">Connexion aux partages SMB :</mark>
   * `smbclient //<cible>/<partage> -U <utilisateur>%<mot_de_passe>` : Connexion à un partage SMB en utilisant un nom d'utilisateur et un mot de passe.
5. <mark style="color:yellow;">Analyse des utilisateurs via SMB :</mark>
   * `enum4linux -U //<cible>` : Liste des utilisateurs via SMB.
6. <mark style="color:yellow;">Récupération de fichiers via SMB :</mark>
   * `smbclient //<cible>/<partage> -U <utilisateur>%<mot_de_passe> -c 'get <fichier_local> <fichier_distant>'` : Récupérer un fichier distant vers un fichier local.
7. <mark style="color:yellow;">Analyse des groupes via SMB :</mark>
   * `enum4linux -G //<cible>` : Liste des groupes via SMB.
8. <mark style="color:yellow;">Récupération du SID (Security Identifier) du domaine :</mark>
   * `rpcclient -U <utilisateur>%>mot_de_passe> -c 'lsaquery' //<cible>` : Récupérer le SID du domaine.
9. <mark style="color:yellow;">Analyse des politiques du domaine :</mark>
   * `rpcclient -U <utilisateur>%<mot_de_passe> -c 'lsadump policy' //<cible>` : Afficher les politiques du domaine.
10. <mark style="color:yellow;">Exploitation de vulnérabilités connues :</mark>
    * Metasploit : Utiliser des modules d'exploitation SMB spécifiques pour cibler des vulnérabilités connues.
