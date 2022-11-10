# Prox-eh

Currently hosted on a 1vCPU 512mb RAM Ubuntu 22.10 x64 droplet on DigitalOcean.

Setup Tailscale:

```shell
curl -fsSL https://tailscale.com/install.sh | sh
sudo tailscale up --auth-key "<auth key>" --hostname "prox-eh" --ssh
```

Setup UFW:

```shell
sudo apt install ufw
sudo ufw default deny incoming
sudo ufw default allow outgoing
sudo ufw allow in on tailscale0
sudo ufw allow http
sudo ufw allow https
sudo ufw enable
```
