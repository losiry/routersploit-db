# HTTP Digest Default Creds

## Description
Module perform dictionary attack with default credentials against HTTP Digest Auth service.

## Authors
* Marcin Bury <marcin.bury[at]reverse-shell.com> # routersploit module

## Usage
```
rsf > use creds/http_digest_default
rsf (HTTP Digest Default Creds) > show options

Target options:

   Name       Current settings     Description
   ----       ----------------     -----------
   target                          Target IP address or file with target:port (file://)
   port       80                   Target port


Module options:

   Name                Current settings                                                              Description
   ----                ----------------                                                              -----------
   threads             8                                                                             Number of threads
   defaults            file:///Users/lucyoa/git/routersploit/routersploit/wordlists/defaults.txt     User:Pass or file with default credentials (file://)
   stop_on_success     1                                                                             Stop on first valid authentication attempt
   path                /                                                                             URL Path
   verbosity           1                                                                             Display authentication attempts


rsf (HTTP Digest Default Creds) > set target http://192.168.1.1
[+] {'target': 'http://192.168.1.1'}
rsf (HTTP Digest Default Creds) > run
[*] Running module...
```
