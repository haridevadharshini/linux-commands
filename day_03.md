# Day 03 – Networking and Wireless Commands

## ifconfig
Displays network interface configuration such as IP address and MAC address.
(Deprecated but still commonly used)

## ip a
Modern replacement for ifconfig.
Shows IP addresses and interface details.

## ping
Checks connectivity between the system and another host.
Example:
ping google.com

## arp -a
Displays the ARP table mapping IP addresses to MAC addresses.

## netstat -ano
Shows active network connections and listening ports.

## route
Displays the system routing table.

## ip r
Modern command to view routing information.

## iwconfig
Used to configure and display wireless network interfaces.

Common uses:
- Check wireless interface details
- View SSID, frequency, and signal strength

Note:
iwconfig is mainly used for wireless interfaces and may not show output on systems without Wi-Fi adapters.
