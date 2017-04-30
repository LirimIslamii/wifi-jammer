# wifi-jammer
This is a Python automated tool to jam all wifi clients within range and disconnect them from their AP. 
Starting with available Wifi networks discovery, It injects Deauthenticaton packets to BSSID. 
Theory behind this
As we know, to disconnect from a connected wifi AP, we have to send an Deauth packet to the AP. Here, we will send a false Deauth packet in which 
the source MAC address is the MAC of the device that we want to jam on it (broadcast to disconnect all wifi clients) and the target is the BSSID's MAC.
We need to set our wifi card on the monitor mode, and we will use scapy to send packets. 
 


