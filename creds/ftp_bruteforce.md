# FTP Bruteforce

## Description
Module performs bruteforce attack against FTP service. If valid credentials are found, they are displayed to the user.

## Authors
* Marcin Bury <marcin.bury[at]reverse-shell.com> # routersploit module

## Usage
```
rsf > use creds/ftp_bruteforce
rsf (FTP Bruteforce) > show options

Target options:

   Name       Current settings     Description
   ----       ----------------     -----------
   target                          Target IP address or file with target:port (file://)
   port       21                   Target port


Module options:

   Name                Current settings                                                               Description
   ----                ----------------                                                               -----------
   usernames           admin                                                                          Username or file with usernames (file://)
   passwords           file:///Users/lucyoa/git/routersploit/routersploit/wordlists/passwords.txt     Password or file with passwords (file://)
   threads             8                                                                              Number of threads
   stop_on_success     yes                                                                            Stop on first valid authentication attempt
   verbosity           yes                                                                            Display authentication attempts


rsf (FTP Bruteforce) > set target 192.168.1.1
[+] {'target': '192.168.1.1'}
rsf (FTP Bruteforce) > run
[*] Running module...
```
