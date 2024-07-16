Mininet-sec is an emulation platform for studying and experimenting cybersecurity in programmable networks. Mininet-Sec allows rapidly prototyping of cybersecurity scenarios, attack simulation and testing offensive security tools in an isolated and secure environment. The availability of specialized resources, along with support for network programmability, enables fast, effective and skilled development of security solutions.

# Overview

The following picture illustrates the overall Mininet-Sec architecture.

![Mininet-Sec big picture](/assets/img/mininet-sec-bigpic.png){:.centered}

The main characteristics are presented below:

- **Network services emulation**: One of Mininet-Sec characteristics is the emulation of common applications or network services, which helps on the service composition to build experiments on offensive and defensive cybersecurity. Web server, e-mail service (SMTP, POP, IMAP), DNS, LDAP, NTP, are some examples of the more than 20 services available on Mininet-Sec.
- **Node library**: another resource available on Mininet-Sec is the possibility of instantiating and using specific cybersecurity services and tools, such as: network Firewalls (based on Netfilter/IPTables), SoftTAPs (for traffic mirroring), P4 switches, Routers, etc.
- **Topology visualization and management**: topology visualization feature allows a easy management of the scenario, identification of link endpoints, remote command execution in some topology equipment, and dynamic addition/removal of components (switches, firewalls, routers, links)
- **Traffic generator**: Mininet-Sec includes tools to support the experimenter for benign traffic generation: [D-ITG](https://sources.debian.org/src/d-itg/) e [TRex](https://trex-tgn.cisco.com).


# Additional information

 - [Getting started](./getting-started.html)
 - [Publications](./publications.html)
 - [Technical guides](./technical-guides.html)
 - [Mininet-Sec team](./team.html)
 - [Source code and Licensing](./source-code-license.html)

# Support

Have you found a bug or wants to request a feature? [Open an issue!](https://github.com/mininet-sec/mininet-sec/issues)

To contact our team, send an e-mail to **mininet-sec [AT] googlegroups.com**.
