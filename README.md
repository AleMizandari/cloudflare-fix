

## What does ufw.sh allow:
* Gets the latest IPv4 and IPv6 lists from Cloudflare. Every week they change their IPs and therefore new information needs to be added every week.

* ufw allow ssh and ufw allow ftp - tells the firewall not to set limits on SSH and FTP ports

* Reads the list and adds cloudflare IP addresses one by one to the UFW whitelist.


## Before running this script, these commands must be written:
* Open command prompt 
## Then type 
* ssh root@ {ip} 
* Password: 

## Do the commands before running the program
* sudo su
* chmod +x ./ufw.sh 
* ufw default deny incoming
* ufw default allow outgoing
* ufw allow from 192.168.1.0/24
* ufw enable
* ./ufw.sh
