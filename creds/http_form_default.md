# HTTP Form Default Creds

## Description
Module performs dictionary attack with default credentials against HTTP form service. If valid credentials are found, they are displayed to the user.

## Authors
* Marcin Bury <marcin.bury[at]reverse-shell.com> # routersploit module

## Usage
```
rsf > use creds/http_form_default
rsf (HTTP Form Default Creds) > show options

Target options:

   Name       Current settings     Description
   ----       ----------------     -----------
   target                          Target IP address or file with target:port (file://)
   port       80                   Target port


Module options:

   Name                Current settings                                                              Description
   ----                ----------------                                                              -----------
   threads             8                                                                             Number of threads
   form                auto                                                                          Post Data: auto or in form login={{USER}}&password={{PASS}}&submit
   stop_on_success     yes                                                                           Stop on first valid authentication attempt
   defaults            file:///Users/lucyoa/git/routersploit/routersploit/wordlists/defaults.txt     User:Pass or file with default credentials (file://)
   verbosity           yes                                                                           Display authentication attempts
   path                /login.php                                                                    URL Path
   form_path           same                                                                          same as path or URL Form Path


rsf (HTTP Form Default Creds) > set target http://192.168.1.1
[+] {'target': 'http://192.168.1.1'}
rsf (HTTP Form Default Creds) > run
[*] Running module...
```
