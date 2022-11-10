# Murai

Currently hosted on a Raspberry Pi 3b+ running RPi OS Lite x64.

Setup Tailscale:

```shell
curl -fsSL https://tailscale.com/install.sh | sh
sudo tailscale up --auth-key "<auth key>" --hostname "murai" --ssh
```
