# Official LAMP Container on EdenServers

[![Run on EdenServers](https://img.shields.io/badge/EdenServers-view-blue.svg)](http://www.edenservers.us)
[![](https://badge.imagelayers.io/edenservers/lamp:latest.svg)](https://imagelayers.io/?images=edenservers/lamp:latest 'Get your own badge on imagelayers.io')

![](http://image.noelshack.com/fichiers/2015/35/1440781181-lamp.jpg)

All-in-one LAMP Server Container built for [EdenServers](http://www.edenservers.us).

It also includes an SCP server.

---

**This image is meant to be used on an EdenServers Server.**

Our images are built to specifically run for our services. You can run it directly with Docker though.

---
### 1.0.0 (2015-08-28)

This initial version contains:

* *LAMP*
* *scp* Server to upload and download files
* *mysql*

---

## Install

    $ docker pull edenservers/lamp

---

## Config

| Environment Variable  | Description |
| ------------- | ------------- |
| USERNAME    | SCP Username  |
| PASSWORD     | SCP Password  |

| Port  | Description |
| ------------- | ------------- |
| 80 | LAMP  |
| 22 | SCP  |

---

## Run example

    $  docker run -p 80:80 -p 1234:22 -e USERNAME=edenservers -e PASSWORD=edenservers --name lamp -d edenservers/lamp

MySQL Infos :
* **database name** : edenservers
* **username** : edenservers
* **password** : edenservers
* **host** : localhost

---

Made by [![EdenServers](http://image.noelshack.com/fichiers/2015/35/1440630894-logo.png)](https://www.edenservers.us)
