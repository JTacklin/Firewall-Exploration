# Firewall-Exploration

This lab follows seed lab's "Linux Firewall Exploration Lab" 

<h2> Setting basic firewall rules in Linux </h2>
We first set up the firewall rules so that our two virtual machines, A and B, cannot connect using 

```sudo ufw deny out from (A ip address) to (B ip address) port 23```

*port 23 being telnet

- You can check if this was successful by using the (telnet) command + the ip you are trying to connet to

<h2>Implementing firewall using Netfilter</h2>

A simple firewall will be imlemented using loadable kernal modules (LKM) and Netfilter.

- You can implement the module using the telnetFilter.c file using the following command

```sudo insmod telnetFilter.ko```

<h2 color=red>Getting around firewalls</h2>

Through a process called SSH tunneling we can get around network blockages to external servers.





