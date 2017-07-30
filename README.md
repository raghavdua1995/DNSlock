# DNSlock - DNSmasq based network wide content/advertisement blocker for debian based operating systems.

###### DNSlock is a DNS forwarder which can block content/advertisement/domains in your whole network

#### --> Installation

Single command Installer:

1) Make sure the device or server on which you want to install DNSlock have a static IP address.
2) Get root permissions (sudo su)
3) `curl https://raw.githubusercontent.com/raghavdua1995/DNSlock/master/install | bash`
4) Configure your devices/router(for network wide content blocking) to use DNSlock as it's primary DNS server

Note : The above installer downloads this [script](https://github.com/raghavdua1995/DNSlock/blob/master/install).

#### --> Commands

DNSlock uses the following commands: 

`DNSlock --update` : Update the hosts file 

`DNSlock --start` : Start DNSlock

`DNSlock --status` : Check if DNSlock is active or inactive

`DNSlock --stop` : Stop DNSlock

`DNSlock --restart` : Restart DNSlock

`DNSlock --blacklist <domain1> <domain2> ..... ` : Blacklist domains 

`DNSlock --*blacklist <domain1> <domain2> ..... ` : Remove domains from blacklist

`DNSlock --whitelist <domain1> <domain2> ..... ` : Whitelist domains

`DNSlock --*whitelist <domain1> <domain2> ..... ` : Remove domains from whitelist

`DNSlock --wildcard <domain1> <domain2> ..... ` : Wildcard block domains

`DNSlock --*wildcard <domain1> <domain2> ..... ` : Remove domains from wildcard list

`DNSlock --tail` : Tail DNSlock logs

`DNSlock --flush` : Flush DNSlock logs

`DNSlock --query` : Query if a domain is being blocked`

#### --> Hosts file sources

DNSlock's hosts file sources are mentioned in /etc/DNSlock/sources.list
You can edit the file and add new sources using any text editor, we will be using nano editor in the following instructions:

1) `sudo nano /etc/DNSlock/sources.list` , Enter password if prompted.
2) Add link for the hosts file you want to add.
3) `DNSlock --update` , Update hosts file

#### --> Uninstallation

Single command Uninstaller:

1) Get root permissions (sudo su)
2) `curl https://raw.githubusercontent.com/raghavdua1995/DNSlock/master/uninstall | bash`
3) Configure your devices/router(for network wide content blocking) to use some other DNS server (like the one provided by your ISP or Google's DNS server).

Note : The above uninstaller downloads this [script](https://github.com/raghavdua1995/DNSlock/blob/master/uninstall).

---
<p align="center">An open source project by <a href="https://raghavdua.in" target="_blank">Raghav Dua</a>.<p>
