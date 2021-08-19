README
======

Superhornet is a shell script to activate hardened Firefox browser mode aka superhornet.

Requirements
------------

- Mozilla Firefox browser (recent release recommended)
- superhornet 

Optional:

- firejail (apt-get install firejail)

To start superhornet in firejail mode:

$ /usr/bin/firejail --x11 --noprofile --private-tmp --allusers --dns=8.8.8.8 /usr/local/bin/superhornet

To start normally:

$ superhornet

Enjoy responsibly! :)

