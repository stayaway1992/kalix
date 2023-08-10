---
description: Énumération SMTP - Cheatsheet
---

# SMTP



1. <mark style="color:yellow;">Découverte des hôtes SMTP :</mark>
   * `nmap -p 25 <cible>` : Scan du port SMTP (port 25) sur un hôte.
2. <mark style="color:yellow;">Vérification de la connectivité SMTP :</mark>
   * `telnet <cible>` 25 : Vérifier la connectivité au serveur SMTP.
3. <mark style="color:yellow;">Requête de service SMTP :</mark>
   * `EHLO <domaine>` : Identifier le domaine de l'émetteur pour l'interaction SMTP (commande SMTP).
   * `HELO <domaine>` : Identifier le domaine de l'émetteur (commande ESMTP).
4. <mark style="color:yellow;">Vérification des utilisateurs (VRFY) :</mark>
   * `VRFY <utilisateur>` : Vérifier si un utilisateur existe sur le serveur.
5. <mark style="color:yellow;">Vérification des boîtes aux lettres (EXPN) :</mark>
   * `EXPN <boîte_aux_lettres>` : Vérifier l'existence d'une boîte aux lettres sur le serveur.
6. <mark style="color:yellow;">Enumération des listes de diffusion (MAIL FROM) :</mark>
   * `RCPT TO:<liste_de_diffusion>` : Vérifier l'existence d'une liste de diffusion.
7. <mark style="color:yellow;">Test d'envoi de courrier électronique :</mark>
   * `MAIL FROM:<adresse_emetteur>` : Indiquer l'adresse de l'émetteur.
   * `RCPT TO:<adresse_destinataire>` : Indiquer l'adresse du destinataire.
   * DATA : Commencer le transfert du courrier électronique.
   * Saisir le corps du message, suivi de "." pour terminer l'envoi.
8. <mark style="color:yellow;">Utilisation de scripts SMTP :</mark>
   * swaks : Outil en ligne de commande pour tester les serveurs SMTP (test d'envoi de courrier électronique).
