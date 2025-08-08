## Access/Block port in kali linux

## step by step commands Used

1. sudo apt update 
2. sudo apt install ufw -y
3. sudo ufw allow 22/tcp (alowing port 22)
4. sudo ufw enable 
5. sudo ufw status verbose (to check our status)

## Allow ports for single Ip or Subnet

> sudo ufw allow from 192.168.xx.xx to any port xx proto tcp 
> sudo ufw allow from 192.168.xx.xx/xx to any port 22 tcp

## Disable port (if we want)

> sudo ufw delete allow 22/tcp

## Command - purpose
ufw enable - start firewall
ufw status verbose - View current rules
ufw deny 23/tcp - Block Telnet
ufw allow 80/tcp - Allow HTTP