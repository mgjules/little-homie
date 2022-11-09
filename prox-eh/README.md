# Prox-eh

Currently hosted on a 1vCPU 512mb RAM Ubuntu 22.10 x64 droplet on DigitalOcean.

Do not forget to setup ufw:
```shell
$ sudo apt install ufw
$ sudo ufw default deny incoming
$ sudo ufw default allow outgoing
$ sudo ufw allow ssh
$ sudo ufw allow http
$ sudo ufw allow https
$ sudo ufw enable
```