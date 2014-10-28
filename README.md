password-utils
==============

This repository contains a small collection of python scripts for managing passwords on multiple *nix servers.



login-chk
---------

Verify an account login works on multiple hosts.  
Create a plain text file with each server on a new line that you want to check your login against.

Example:

    $ login-chk all_servers.txt
    Username: username
    Password:
    Confirm Password:
    Successfully logged in to:  yourserver1.com
    Successfully logged in to:  yourserver2.com
  
Dependencies:  
pexpect - http://sourceforge.net/projects/pexpect/


pupd
---------

Change a users password on multiple hosts.  
Create a plain text file with each server on a new line that you want to change your password.

Example:

    $ pupd servers_test.txt
    Username: username
    Current Password:
    New Password:
    Confirm New Password:
    Changed password on host:  yourserver1.com
    Changed password on host:  yourserver2.com
  
Dependencies:  
pexpect - http://sourceforge.net/projects/pexpect/
sudo access required



Problems
--------

Please report any issue/suggestions via the github repository:

* https://github.com/ericglass/password-utils


Author
------

Eric Glass <ericcglass@gmail.com>
