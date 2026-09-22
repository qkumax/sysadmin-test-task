
# 2. Remote Access

## SSH Key Authentication

ED25519 key, passwordless login:

    ssh test123@10.0.10.1

## WireGuard VPN

- Server: `wg0` — 10.8.0.1/24, port 51820
- Client: `wg-client` — 10.8.0.2/24
- Configs: `/etc/wireguard/wg0.conf`, `/etc/wireguard/wg-client.conf`
- Autostart: `systemctl enable wg-quick@wg0 wg-quick@wg-client`

### Verification

    sudo wg show
    ping -c 3 10.8.0.1

Result: `latest handshake: Now`, transfer > 0, ping 0% loss.

Screenshots: `../screenshots/2-wireguard-status.png`, `../screenshots/2-wireguard-ping.png`, `../screenshots/2-ssh.png`
