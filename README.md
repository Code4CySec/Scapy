#Scapy, a powerfull Python library. Here you'll find scripts to help you understant network traffic capture, MITM attacks, credential theft, ARP poisoning and more.

- email_sniffer_structure.py

In this first script, we write the fundamentals of an email sniffer. This would be the skelleton of a well written email sniffer, this should help you understand it better the structure of the sniffer.

- email_sniffer.py

This is a more structured script to sniff the network for credentials. This script will sniff only the packets we are interested, like a packet filter. 

- arper.py

  ARP poisoning is a very effective type of attack, and also one of the oldest ones. Which means all traffic in the victim's computer has to go through you first.
  To start this attack first you need to forward the IP, in your Kali VM enter the command:

  echo 1 > /proc/sys/net/ipv4/ip_forward

  Now you are ready to run the arper.py script and start capturing traffic

  sudo arper.py "Target IP" 192.168.1.254 eth0
