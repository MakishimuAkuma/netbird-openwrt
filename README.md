# netbird-openwrt

### Install trust key once

```sh
wget -qO /etc/apk/keys/netbird-feed.pem https://raw.githubusercontent.com/MakishimuAkuma/netbird-openwrt/gh-pages/netbird-feed.pub.pem
```

### Add repository

```sh
echo 'https://raw.githubusercontent.com/MakishimuAkuma/netbird-openwrt/gh-pages/25.12/<ARCH>/packages.adb' > /etc/apk/repositories.d/netbird.list
apk update
apk add netbird
```

### Update NetBird

```sh
apk update
apk upgrade netbird
```
