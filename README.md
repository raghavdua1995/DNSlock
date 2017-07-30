DNSlock
----------

DNSmasq based network wide content/advertisement blocker for debian based operating system.
----------
DNSlock is a DNS forwarder which can block content/advertisement/domains in your whole network

Installation
Single command Installer:
1) Make sure the device or server on which you want to install DNSlock have a static IP address.
2) Get root permissions (sudo su)
3) `curl https://raw.githubusercontent.com/raghavdua1995/DNSlock/master/install | bash`
4) Configure your devices/router(for network wide content blocking) to use DNSlock as it's primary DNS server

Note : The above installer downloads this [script](https://github.com/raghavdua1995/DNSlock/blob/master/install).

Commands
DNSlock uses the following command: 

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

Uninstallation
Single command Uninstaller:
1) Get root permissions (sudo su)
2) `curl https://raw.githubusercontent.com/raghavdua1995/DNSlock/master/uninstall | bash`
3) Configure your devices/router(for network wide content blocking) to use some other DNS server (like the one provided by your ISP or Google's DNS server).

Note : The above installer downloads this [script](https://github.com/raghavdua1995/DNSlock/blob/master/uninstall).
