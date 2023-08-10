---
description: Scripting et commandes en powershell, les bases
---

# Basic Powershell

1. <mark style="color:yellow;">Découverte du Réseau :</mark>
   * Test-NetConnection -ComputerName example.com -Port 80 : Tester la connectivité à example.com sur le port 80.
   * Resolve-DnsName www.example.com : Résoudre l'adresse IP de www.example.com.
2. <mark style="color:yellow;">Enumération du Réseau :</mark>
   * Get-NetTCPConnection : Afficher les connexions TCP en cours.
   * Get-NetUDPEndpoint : Afficher les connexions UDP en cours.
   * Get-NetRoute : Afficher les tables de routage du système.
3. <mark style="color:yellow;">Analyse de Vulnérabilités :</mark>
   * Test-Path C:\Windows\System32\cmd.exe : Vérifier si le fichier cmd.exe existe sur le système.
   * Get-Process : Afficher les processus en cours d'exécution.
   * Get-Service -DisplayName "Windows Firewall" : Afficher l'état du service Pare-feu Windows.
4. <mark style="color:yellow;">Exploitation :</mark>
   * Invoke-Command -ComputerName target -ScriptBlock { Get-Process } : Exécuter Get-Process à distance sur l'ordinateur "target".
   * New-Object -ComObject Shell.Application : Créer un objet pour l'interaction avec l'application Shell.
   * (New-Object System.Net.WebClient).DownloadFile("http://example.com/monfichier.txt", "C:\temp\monfichier.txt") : Télécharger un fichier depuis un serveur distant.
5. <mark style="color:yellow;">Persistence :</mark>
   * New-Item -Path "HKCU:\SOFTWARE\Microsoft\Windows\CurrentVersion\Run" -Name "MonScript" -Value "C:\Chemin\MonScript.ps1" : Ajouter un script dans la clé de registre "Run" pour s'exécuter au démarrage.
   * New-Service -Name "MonService" -BinaryPathName "C:\Chemin\MonScript.ps1" -DisplayName "Mon Service" : Créer un service basé sur un script PowerShell.
6. <mark style="color:yellow;">Capture de Mots de Passe :</mark>
   * Get-Credential : Afficher une boîte de dialogue pour saisir des informations d'identification.
7. <mark style="color:yellow;">Utilitaires pour Pentest :</mark>
   * PowerSploit : Import-Module PowerSploit pour utiliser les outils PowerShell pour les tests d'intrusion.
   * Empire : Import-Module Empire pour utiliser le cadre pour l'administration post-exploitation en PowerShell.
   * Invoke-Obfuscation : Invoke-Obfuscation -ScriptBlock { Get-Process } pour obfusquer le script Get-Process.
8. <mark style="color:yellow;">Sécurité :</mark>
   * Set-ExecutionPolicy RemoteSigned : Définir la politique d'exécution pour autoriser l'exécution des scripts locaux signés et des scripts distants non signés.
   * Set-ExecutionPolicy Bypass -Scope Process : Définir la politique d'exécution pour permettre l'exécution de scripts non signés uniquement dans la session actuelle.
