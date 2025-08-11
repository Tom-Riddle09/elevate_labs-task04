# Elevate Labs - Task 04

## Objective
 Configure and test basic firewall rules to allow or block traffic.  

 ## Tools Used
OS : Linux Debian, Windows 11
UFW (Uncomplicated Firewall)  
SSH, Telnet, CMD

## Commands Used
-> Install & Enable UFW Firewall:  
sudo apt install ufw  
sudo ufw enable  
-> Block Telnet : sudo ufw deny 23  
-> Allow SSH: sudo ufw allow 22  
-> Delete Telnet block rule: sudo ufw delete deny 23  

 ## Results 
 -> Tested UFW rules by connecting from Windows host  
telnet 192.168.1.10 23 |  Telnet connection failed.  
ssh nessus-vm@192.168.1.10 | SSH connection was successful.  

## Documented Screenshots
1. UFW status before adding rules.
2. Telnet connection testing.
3. SSH connection testing.
4. UFW status after adding rules.

## Summarize how firewall filters traffic
Firewall filters traffic by matching rules against packet headers and dropping or allowing accordingly.
