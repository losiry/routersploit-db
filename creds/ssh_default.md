# SSH Default Creds

## Description
Module perform dictionary attack with default credentials against SSH service. If valid credentials are found, they are displayed to the user.

## Authors
* Marcin Bury <marcin.bury[at]reverse-shell.com> # routersploit module

## Usage
```
rsf > use creds/ssh_default
rsf (SSH Default Creds) > show options

Target options:

   Name       Current settings     Description
   ----       ----------------     -----------
   target                          Target IP address or file with target:port (file://)
   port       22                   Target port


Module options:

   Name                Current settings                                                              Description
   ----                ----------------                                                              -----------
   threads             8                                                                             Numbers of threads
   defaults            file:///Users/lucyoa/git/routersploit/routersploit/wordlists/defaults.txt     User:Pass or file with default credentials (file://)
   stop_on_success     yes                                                                           Stop on first valid authentication attempt
   verbosity           yes                                                                           Display authentication attempts


rsf (SSH Default Creds) > set target 192.168.1.1
[+] {'target': '192.168.1.1'}
rsf (SSH Default Creds) > run
[*] Running module...
```
