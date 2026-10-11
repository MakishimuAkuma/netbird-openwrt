# netbird-openwrt 25.12+

### Install trust key once

```sh
wget -qO "/etc/apk/keys/netbird-feed.pem" "https://makishimuakuma.github.io/netbird-openwrt/netbird-feed.pub.pem"
```

### Add repository

```sh
echo "https://makishimuakuma.github.io/netbird-openwrt/25.12/$(cat /etc/apk/arch)/packages.adb" > "/etc/apk/repositories.d/netbird.list"
apk update
apk add netbird
```

### Update NetBird

```sh
apk update
apk upgrade netbird
```
