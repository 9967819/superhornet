Superhornet is a shell script to activate headless Firefox browser mode aka superhornet.

Basic requirements:

1. Mozilla Firefox or Waterfox browser (recent release recommended)

2. superhornet script included in the repo

Optional libraries:

- firejail (apt-get install firejail)
- Xephyr library (experimental, untested) : dnf install xorg-x11-server-Xephyr



Usage:

First copy superhornet to /usr/local/bin:
sudo cp superhornet /usr/local/bin/

To start superhornet in firejail mode:
$ firejail --x11 --noprofile --private-tmp --allusers --dns=8.8.8.8 /usr/local/bin/superhornet

Alternatively you can use firejail-superhornet wrapper:
$ firejail-superhornet 

To start normally:
$ /usr/local/bin/superhornet


See also:

firejail(8) 


Known issues:

1. firejail segfault with --memory-deny-write-execute


Have fun! :)
