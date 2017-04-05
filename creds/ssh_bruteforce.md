# SSH Bruteforce

## Description
Module performs bruteforce attack against SSH service. If valid credentials are found, they are displayed to the user.

## Authors
* Marcin Bury <marcin.bury[at]reverse-shell.com> # routersploit module

## Usage
```
rsf > use creds/ssh_bruteforce
rsf (SSH Bruteforce) > show options

Target options:

   Name       Current settings     Description
   ----       ----------------     -----------
   target                          Target IP address or file with target:port (file://)
   port       22                   Target port


Module options:

   Name                Current settings                                                               Description
   ----                ----------------                                                               -----------
   usernames           admin                                                                          Username or file with usernames (file://)
   passwords           file:///Users/lucyoa/git/routersploit/routersploit/wordlists/passwords.txt     Password or file with passwords (file://)
   threads             8                                                                              Number of threads
   stop_on_success     yes                                                                            Stop on first valid authentication attempt
   verbosity           yes                                                                            Display authentication attempts


rsf (SSH Bruteforce) > set target 192.168.1.1
[+] {'target': '192.168.1.1'}
rsf (SSH Bruteforce) > run
[*] Running module...
```
