# 3X-UI

**An Advanced Web Panel • Built on Xray Core**

[![](https://img.shields.io/github/v/release/phuonganh2601/3x-ui.svg)](https://github.com/phuonganh2601/3x-ui/releases)
[![](https://img.shields.io/github/actions/workflow/status/phuonganh2601/3x-ui/release.yml.svg)](#)
[![GO Version](https://img.shields.io/github/go-mod/go-version/phuonganh2601/3x-ui.svg)](#)
[![Downloads](https://img.shields.io/github/downloads/phuonganh2601/3x-ui/total.svg)](#)
[![License](https://img.shields.io/badge/license-GPL%20V3-blue.svg?longCache=true)](https://www.gnu.org/licenses/gpl-3.0.en.html)

## Install & Upgrade

```
bash <(curl -Ls https://raw.githubusercontent.com/phuonganh2601/3x-ui/custom/install.sh)
```

## Install with Docker

 ```sh
 docker run -itd \
    -e XRAY_VMESS_AEAD_FORCED=false \
    -e TZ=Asia/Ho_Chi_Minh \
    -v $PWD/db/:/etc/x-ui/ \
    -v $PWD/cert/:/root/cert/ \
    --network=host \
    --restart=unless-stopped \
    --name 3x-ui \
    ghcr.io/phuonganh2601/3x-ui:latest
 ```

## Default Settings

- **Port:** 2053
- **Username & Password:** It will be generated randomly if you skip modifying.
- **Database Path:**
  - /etc/x-ui/x-ui.db
- **Xray Config Path:**
  - /usr/local/x-ui/bin/config.json
- **Web Panel Path w/o Deploying SSL:**
  - http://ip:2053/panel
  - http://domain:2053/panel
- **Web Panel Path w/ Deploying SSL:**
  - https://domain:2053/panel
