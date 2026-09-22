

**Окружение:** Ubuntu Server 26.04.1, VirtualBox, интерфейс `enp0s3` (NAT).

## Адресация

| Интерфейс | VLAN | IP |
|---|---|# 1. Настройка сети

**Окружение:** Ubuntu Server 26.04.1, VirtualBox, интерфейс `enp0s3` (NAT).

## Адресация

| Интерфейс | VLAN | IP |
|---|---|---|
| enp0s3 | — | 10.0.2.15/24 (DHCP) |
| enp0s3.10 | 10 | 10.0.10.1/24 |
| enp0s3.20 | 20 | 10.0.20.1/24 |

## Конфиг `/etc/netplan/01-vlan-config.yaml`

```yaml
network:
  version: 2
  renderer: networkd
  ethernets:
    enp0s3:
      dhcp4: true
      dhcp6: false
  vlans:
    enp0s3.10:
      id: 10
      link: enp0s3
      addresses: [10.0.10.1/24]
    enp0s3.20:
      id: 20
      link: enp0s3
      addresses: [10.0.2| enp0s3 | — | 10.0.2.15/24 (DHCP) |
| enp0s3.10 | 10 | 10.0.10.1/24 |
| enp0s3.20 | 20 | 10.0.20.1/24 |

## Конфиг `/etc/netplan/01-vlan-config.yaml`

```yaml
network:
  version: 2
  renderer: networkd
  ethernets:
    enp0s3:
      dhcp4: true
      dhcp6: false
  vlans:
    enp0s3.10:
      id: 10
      link: enp0s3
      addresses: [10.0.10.1/24]
    enp0s3.20:
      id: 20
      link: enp0s3
      addresses: [10.0.20.1/24]
