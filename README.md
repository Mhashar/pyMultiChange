pyMultiChange
=============

It utilizes a python library called 'netlib' The latest version of 'netlib' can be obtained at:

https://github.com/jtdub/netlib

Netlib is also included as a submodule and can be obtained via the git
submodule commands.

    git submodule init
    git submodule update
    cd netlib
    git pull

    sudo pip install -r netlib/requirements.txt

PyMultiChange is a script that allows you to make mass changes to cisco routers and switches.

## multi.py

```
usage: multi.py [-h] -d DEVICES -c COMMANDS [-s [SSH]] [-t [TELNET]]
                [-o [OUTPUT]] [-v [VERBOSE]] [--delay DELAY] [--buffer BUFFER]
                [--threaded [THREADED]] [-m MAXTHREADS]

Managing network devices with python

optional arguments:
  -h, --help            show this help message and exit
  -d DEVICES, --devices DEVICES
                        Specifies a host file
  -c COMMANDS, --commands COMMANDS
                        Specifies a commands file
  -s [SSH], --ssh [SSH]
                        Default: Use the SSH protocol
  -t [TELNET], --telnet [TELNET]
                        Use the Telnet protocol
  -o [OUTPUT], --output [OUTPUT]
                        Verbose command output
  -v [VERBOSE], --verbose [VERBOSE]
                        Debug script output
  --delay DELAY         Change the default delay exec between commands
  --buffer BUFFER       Change the default SSH output buffer
  --threaded [THREADED]
                        Enable process threading
  -m MAXTHREADS, --maxthreads MAXTHREADS
                        Define the maximum number of threads
```
