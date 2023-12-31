# Table of contents

* [⌚ Kalix's Notebook](README.md)
* [Méthodologie](methodologie.md)
* [Enumeration](enumeration/README.md)
  * [Utilisation de nmap](enumeration/utilisation-de-nmap.md)
  * [SSH](enumeration/ssh.md)
  * [HTTP](enumeration/http.md)
  * [FTP](enumeration/ftp.md)
  * [SMB](enumeration/smb.md)
  * [SMTP](enumeration/smtp.md)
  * [SQL](enumeration/sql.md)
  * [Liste des ports communs](enumeration/liste-des-ports-communs.md)
* [Scan de Vulnérabilités](scan-de-vulnerabilites/README.md)
  * [Nessus](scan-de-vulnerabilites/nessus.md)
  * [Nmap Script Engine](scan-de-vulnerabilites/nmap-script-engine.md)
  * [Scan de vulnerabilites avec Metasploit](scan-de-vulnerabilites/scan-de-vulnerabilites-avec-metasploit.md)
  * [Banner grabbing avec netcat](scan-de-vulnerabilites/banner-grabbing-avec-netcat.md)
* [Exploitation](exploitation/README.md)
  * [Bind Shell](exploitation/bind-shell.md)
  * [Reverse Shell](exploitation/reverse-shell.md)
  * [Obfuscation de script Powershell](exploitation/obfuscation-de-script-powershell.md)
  * [Compilation cross platform d'exploit](exploitation/compilation-cross-platform-dexploit.md)
  * [Evasion d'AV avec Shellter](exploitation/evasion-dav-avec-shellter.md)
  * [Recherche d'exploits public](exploitation/recherche-dexploits-public.md)
  * [Exploitations communes](exploitation/exploitations-communes.md)
* [Post-Exploitation](post-exploitation/README.md)
  * [Windows](post-exploitation/windows/README.md)
    * [Post Exploitation Windows Enumération](post-exploitation/windows/post-exploitation-windows-enumeration.md)
    * [Abus de Configurations Incorrectes de Services Cheatsheet](post-exploitation/windows/abus-de-configurations-incorrectes-de-services-cheatsheet.md)
    * [Abus de logiciels vulnerables Cheatsheet](post-exploitation/windows/abus-de-logiciels-vulnerables-cheatsheet.md)
    * [Abus de Privileges dangereux Cheatsheet](post-exploitation/windows/abus-de-privileges-dangereux-cheatsheet.md)
    * [Strategie AlwaysInstallElevated](post-exploitation/windows/strategie-alwaysinstallelevated.md)
    * [Extractions de Mots de Passe aux Emplacements Habituels Cheatsheet](post-exploitation/windows/extractions-de-mots-de-passe-aux-emplacements-habituels-cheatsheet.md)
    * [Taches Planifiees Cheatsheet](post-exploitation/windows/taches-planifiees-cheatsheet.md)
    * [Extractions et cracking Windows](post-exploitation/windows/extractions-et-cracking-windows.md)
    * [Persistence Windows](post-exploitation/windows/persistence-windows.md)
  * [Linux](post-exploitation/linux/README.md)
    * [Post Exploitation Linux   Enumeration](post-exploitation/linux/post-exploitation-linux-enumeration.md)
    * [SUID](post-exploitation/linux/suid.md)
    * [SUDO](post-exploitation/linux/sudo.md)
    * [PATH](post-exploitation/linux/path.md)
    * [NFS](post-exploitation/linux/nfs.md)
    * [Kernel Exploits](post-exploitation/linux/kernel-exploits.md)
    * [Cron Jobs](post-exploitation/linux/cron-jobs.md)
    * [Capabilities](post-exploitation/linux/capabilities.md)
    * [Persistence Linux](post-exploitation/linux/persistence-linux.md)
    * [Extractions et cracking Linux](post-exploitation/linux/extractions-et-cracking-linux.md)
  * [Pivotage](post-exploitation/pivotage.md)
  * [Transfert de fichier](post-exploitation/transfert-de-fichier.md)
  * [Upgrade de Shell](post-exploitation/upgrade-de-shell.md)
* [Pentest d'application web](pentest-dapplication-web/README.md)
  * [Scan d'application web Nikto](pentest-dapplication-web/scan-dapplication-web-nikto.md)
  * [Enumeration de dossiers et fichiers](pentest-dapplication-web/enumeration-de-dossiers-et-fichiers.md)
  * [Attaques XSS](pentest-dapplication-web/attaques-xss.md)
  * [Injections SQL](pentest-dapplication-web/injections-sql.md)
  * [HTTP login avec Hydra](pentest-dapplication-web/http-login-avec-hydra.md)
  * [Login avec Burp](pentest-dapplication-web/login-avec-burp.md)
* [Outils](outils/README.md)
  * [Liste exhaustive d'outils pour le pentest](outils/liste-exhaustive-doutils-pour-le-pentest.md)
  * [Masscan](outils/masscan.md)
  * [DNSenum](outils/dnsenum.md)
  * [theHarvester](outils/theharvester.md)
  * [SQLMap](outils/sqlmap.md)
  * [XSSer](outils/xsser.md)
  * [WPscan](outils/wpscan.md)
  * [Netcat](outils/netcat.md)
  * [Mimikatz](outils/mimikatz.md)
  * [Cadaver](outils/cadaver.md)
  * [Windows Exploit Suggester](outils/windows-exploit-suggester.md)
  * [Linux Exploit Suggester](outils/linux-exploit-suggester.md)
  * [LinEnum](outils/linenum.md)
  * [Shred](outils/shred.md)
  * [John](outils/john.md)
  * [Hashcat](outils/hashcat.md)
  * [Impacket](outils/impacket.md)
  * [Burp Suite](outils/burp-suite.md)
  * [Wireshark](outils/wireshark.md)
  * [Autorecon](outils/autorecon.md)
  * [Evil-WinRM](outils/evil-winrm.md)
  * [CrackMapExec](outils/crackmapexec.md)
  * [MSFVenom](outils/msfvenom.md)
  * [Joomscan](outils/joomscan.md)
  * [Binwalk](outils/binwalk.md)
  * [Steghide](outils/steghide.md)
* [OSINT](osint/README.md)
  * [Recherches avancees Google](osint/recherches-avancees-google.md)
* [Scripting](scripting/README.md)
  * [Basic Powershell](scripting/basic-powershell.md)
* [Cryptographie](cryptographie/README.md)
  * [GPG](cryptographie/gpg.md)
* [Cheatsheet ingénierie sociale](cheatsheet-ingenierie-sociale/README.md)
  * [Gophish](cheatsheet-ingenierie-sociale/gophish.md)
* [Cheatsheet Réseaux](cheatsheet-reseaux.md)
* [🖤 README.md](readme.md.md)
* [⚠ Rapports de CTF](rapports-de-ctf.md)
