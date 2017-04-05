# SNMP Bruteforce

## Description
Module performs bruteforce attack against SNMP service. If valid community string is found, it is displayed to the user.

## Authors
* Marcin Bury <marcin.bury[at]reverse-shell.com> # routersploit module

## Usage
```
rsf > use creds/snmp_bruteforce
rsf (SNMP Bruteforce) > show options

Target options:

   Name       Current settings     Description
   ----       ----------------     -----------
   target                          Target IP address or file with target:port (file://)
   port       161                  Target port


Module options:

   Name                Current settings                                                          Description
   ----                ----------------                                                          -----------
   threads             8                                                                         Number of threads
   stop_on_success     yes                                                                       Stop on first valid community string
   verbosity           yes                                                                       Display authentication attempts
   snmp                file:///Users/lucyoa/git/routersploit/routersploit/wordlists/snmp.txt     Community string or file with community strings (file://)


rsf (SNMP Bruteforce) > set target 192.168.1.1
[+] {'target': '192.168.1.1'}
rsf (SNMP Bruteforce) > run
[*] Running module...
```
