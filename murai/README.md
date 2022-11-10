# Murai

Currently hosted on a Raspberry Pi 3b+ running RPi OS Lite x64.

Setup Tailscale:

```shell
curl -fsSL https://tailscale.com/install.sh | sh
sudo tailscale up --auth-key "<auth key>" --hostname "murai" --ssh
```

Setup UFW:

```shell
sudo apt install ufw
sudo ufw default deny incoming
sudo ufw default allow outgoing
sudo ufw allow in on tailscale0
sudo ufw enable
```
