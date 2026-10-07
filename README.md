# netbird-openwrt

### Install trust key once

```sh
wget -qO /etc/apk/keys/netbird-feed.pem ${KEY}
```

### Add repository

```sh
echo '${BASE}/<ARCH>/packages.adb' > /etc/apk/repositories.d/netbird.list
apk update
apk add netbird
```

### Update NetBird

```sh
echo '${BASE}/<ARCH>/packages.adb' > /etc/apk/repositories.d/netbird.list
apk update
apk upgrade netbird
```
