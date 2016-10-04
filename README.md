# Lazy-Cyberoam
#Introduction
 Hotspotd is a small daemon to create a wifi hotspot on linux. It depends on hostapd for AP provisioning and dnsmasq to assign IP addresses to devices.
 
 Hotspotd works by creating a virtual NAT (Network address transation) table between your connected device and the internet using linux iptables.

#Usage
EDIT THE BATCH FILE AND CONFIGURE YOUR USERNAME AND PASSWORD RESPECTIVELY. COMMENT OUT THE LINES FOR HOTSPOT STARTUP AND TERMINATION AS PER REQUIREMENT.
 
Command Line and Python Script for Starting Hotspot and Logging into Cyberoam User Portal

#Troubleshooting 
  Make sure all dependencies (hostapd, dnsmasq and python 2.7) are installed.

  Hotspotd creates the NAT by manipulating iptables rules. So if you have any other firewall software that manipulates the iptables rules (such as the firewalld on fedora), make sure you disable that.

-------------
        NOTE: YOU CAN CHANGE THE URL FOR CYBEROAM HOST IN PYTHON FILE. 
