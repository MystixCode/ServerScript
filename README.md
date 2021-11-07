# ServerScript
Script to install nginx based webserver on a debian 11 server.

Alpha version. Still in development!

## How it works
1. First the script installs nginx and configures ur domains and subdomains with http using normal directory or proxypass.
2. Then u can check if everythings works over the internet with the portforwarding and dns records.
3. After that the script adds https with letsencrypt and h2 configuration.
4. And u can use it to install and configure additional packages like ufw, openssh-server, mariadb and fail2ban.

## Prerequisites
- Debian 11 server
- git
- A domain name configured with dns record to your WAN IP (A or CAA for better security). For example:
  - [empty]  ->  WAN IP
  - www      ->  WAN IP
  - api      ->  WAN IP
  
- On your router: port forwarding for http port 80 and https port 443 to your debian server.

## Installation
```bash
git clone https://github.com/MystixCode/ServerScript.git
cd ServerScript
chmod u+x ServerScript
./Serverscript
```
