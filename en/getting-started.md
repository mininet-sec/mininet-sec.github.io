# Getting started -- Install procedure

Prerequisites
-------------

Mininet-Sec is tested on the following Linux distributions:

- Ubuntu 22.04, 24.04
- Debian 11 (recommended)

You must have sudo privileges to install and run Mininet-Sec.

Using Vagrantfile
-----------------

With Vagrant installed, simply do ``vagrant up`` which will bring up an Debian 11 virtual machine
and install Mininet-Sec and all its dependencies on it. Please make sure to tweak the CPU core count
(default 4 cores) and RAM (default 4GB) according to your needs before doing vagrant up. Mininet-Sec
can be found in /home/vagrant/minet-sec which is a symlink to /mininet-sec if Vagrantfile was used
from within mininet-sec cloned on the host. Otherwise it is an actual clone of mininet-sec.

Using install.sh
----------------

To install Mininet-Sec and its dependencies, clone this repository and run:

::

    git clone https://github.com/mininet-sec/mininet-sec
    ./install.sh

The script accepts various command line flags.
Some notable flags are:

- ``-y`` skips interactive confirmation before installation.
- ``--ppa`` prefers installing software from `PPA <https://launchpad.net/~italovalcy/+archive/debian/ppa>`_.
  This shortens installation time by downloading binary packages, but is only available on Debian.
- ``--source`` prefers installing Mininet-Sec dependencies from source code.

You can see all command line flags by running:

::

    ./install.sh -h

The script uses ``setup.py develop`` to point the system install of Python packages to the codebase
directory. Therefore, you can modify ``mininet``, ``mininet-sec``, and other componets, and the
changes will be reflected immediately.

Verification
------------

You can execute the following example to bring up the Mininet-Sec command line:

::

    sudo python3 examples/firewall.py

You can use these steps to run the sample scan experiment:

1. Issue the command: ``sudo python3 examples/scanall.py``
2. When the ``mnsec>`` CLI prompt appears, the experiment has
   finished. On the Mininet-Sec CLI, issue the command ``exit`` to exit the
   experiment.
3. You should notice an output similar to displayed below:

::

	Starting Nmap 7.80 ( https://nmap.org ) at 2024-06-22 14:50 UTC
	
	Nmap scan report for 10.0.0.1
	Host is up (0.000016s latency).
	Not shown: 998 closed ports
	PORT   STATE SERVICE
	22/tcp open  ssh
	80/tcp open  http
	MAC Address: 22:88:4B:0F:15:D4 (Unknown)
	
	Nmap scan report for 10.0.0.2
	Host is up (0.000013s latency).
	Not shown: 999 closed ports
	PORT    STATE SERVICE
	389/tcp open  ldap
	MAC Address: BA:EE:E2:02:51:33 (Unknown)
	
	Nmap scan report for 10.0.0.3
	Host is up (0.0000040s latency).
	Not shown: 998 closed ports
	PORT    STATE SERVICE
	25/tcp  open  smtp
	143/tcp open  imap
	
	Nmap done: 256 IP addresses (3 hosts up) scanned in 28.33 seconds
