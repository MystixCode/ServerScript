# ServerScript
Script to install nginx based webserver on a debian11 system.

Alpha version. Still in development!

## How it works
1. First the script installs nginx and configures ur domains and subdomains with http using normal directory or proxypass.
2. Then u can check if everythings works over the internet with the portforwarding and dns records.
3. After that the script adds https with letsencrypt and h2 configuration.
4. And u can use it to install and configure additional packages like ufw, openssh-server, mariadb and fail2ban.
