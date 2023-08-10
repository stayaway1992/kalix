---
description: Evil-WinRM - Outil d'Exploitation WinRM
---

# Evil-WinRM

<mark style="color:yellow;">Description :</mark>&#x20;

Evil-WinRM est un shell WinRM ultime conçu pour le hacking et les tests d'intrusion.

WinRM (Windows Remote Management) est la mise en œuvre de Microsoft du protocole WS-Management.

Ce programme peut être utilisé sur n'importe quel serveur Microsoft Windows avec cette fonctionnalité activée (généralement sur le port 5985), mais seulement si vous avez des informations d'identification et des autorisations pour l'utiliser. L'objectif de ce programme est de fournir des fonctionnalités pratiques et faciles à utiliser pour le hacking.&#x20;

<mark style="color:yellow;">Exemples d'utilisation :</mark>

* `evil-winrm -i <adresse_IP> -u <nom_utilisateur> -p <mot_de_passe>` : Se connecter à un hôte distant avec les informations d'identification spécifiées.
* `shell` : Ouvrir un shell interactif sur le système cible.
* `upload <fichier_local> <chemin_cible>` : Transférer un fichier local vers le système cible.
