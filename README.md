# Ad-Blocker-Using-Pi-hole
We can use below method to block advertisement in user devices in whole network using pi-hole

1. Firstly we have to setup ubuntu server.
2. we have to make ip address of ubuntu server as static ip Address by updating 00-installer-config.yaml file.
.. code-block:: console
   sudo nano /etc/netplan/00-installer-config.yaml
   sudo netplan apply
3. make ubuntu server as DNS server after install pi-hole in ubuntu server.
.. code-block:: console
   wget -0 basic-install.sh https://install.pi-hole.net
4. Steps to follow below for setup of another virtual machine.
5. right click on network settings.
6. so to change adapter options.
7. right click on Ethernet0 network adapter and select properties.
8. double click the internet protocol version 4 (TCP/Ipv4) Properties.
9. update DNS server addresses as 192.168.100.248
10. go and access PI-hole 192.168.100.248/admin and login.

Finally we can access web without ads by following above steps.
