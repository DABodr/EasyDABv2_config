# EasyDABv2 configuration 

First use configuration for Debian/Raspbian Jessie:

- sudo nano /etc/network/interfaces
- add this lines:

* auto eth0
* allow-hotplug eth0
* iface eth0 inet static
* address 192.168.2.5
* netmask 255.255.255.0

- sudo service networking restart


For Debian/Raspbian Stretch:

- sudo nano /etc/dhcpcd.conf
- add:

* interface eth0
* static ip_address=192.168.2.5/24
