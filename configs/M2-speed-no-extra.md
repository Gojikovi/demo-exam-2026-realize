# ⏱ Модуль 2 — Быстрый готовый конфиг с командами без лишнего 🔥

## Заточен под реальный стенд на Proxmox в колледже

### 🐧 ISP

```
vim /etc/chrony.conf
local stratum 5
allow 0.0.0.0/0
systemctl enable --now chronyd

```

### 🐧 HQ-CLI

```
apt-get update
apt-get install yandex-browser-stable -y
yandex-browser-stable

apt-get install chrony -y
vim /etc/chrony.conf
#pool pool.ntp.org iburst
server 172.16.4.1 iburst
systemctl enable --now chronyd
chronyc sources

mkdir /mnt/nfs
```

### 🐧 HQ-SRV

```
apt-get update
apt-get install chrony -y
vim /etc/chrony.conf
#pool pool.ntp.org iburst
server 172.16.4.1 iburst
systemctl enable --now chronyd
```

### 🐧 BR-SRV

```

```







### 🍃 HQ-RTR

