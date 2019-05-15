# Break the Fucking GFW

Proxy

* Shadowsocks - SS
  * Server
    * [github](https://github.com/shadowsocks/shadowsocks/tree/master)
  * Client
    * [shadowsocks-libev](https://github.com/shadowsocks/shadowsocks-libev)
      * [openwrt-shadowsocks](https://github.com/shadowsocks/openwrt-shadowsocks)
    * Shadowsocks - Android
    * Shadowrocket - iOS
* [ShadowsocksR](https://github.com/shadowsocksrr) - SSR ([backup](https://github.com/shadowsocksr-backup))
  * Server
    * [backup repo](https://github.com/shadowsocksr-backup/shadowsocksr)
  * Client
    * SSR - Android
    * Shadowrocket - iOS
* [V2Ray](https://github.com/v2ray)
  * Tutorial
    * [official manual](https://www.v2ray.com/en/)
    * [V2Ray 配置指南](https://toutyrater.github.io/)
  * Server
    * [v2ray-core](https://github.com/v2ray/v2ray-core)
  * Client
    * BifrostV - Android

VPN

* [Pulse Secure](https://www.pulsesecure.net/) - usually used by campus VPN
  * [download](https://www.pulsesecure.net/trynow/client-download/)
* Free App
  * iOS
    * VPN Cat
    * VPN Master

Others

* [SwitchyOmega](https://github.com/FelisCatus/SwitchyOmega) - Manage and switch between multiple proxies quickly & easily.

## Shadowsocks

* [mrluanma/shadowsocks-heroku](https://github.com/mrluanma/shadowsocks-heroku)

### Shadowsocks on Debian System

Install

```sh
sudo apt-get install shadowsocks
```

Setting: edit `/etc/shadowsocks/config.json`

Must set:

* server
* server_port
* password
* method

```json
{
    "server":"server_ip",
    "server_port":server_port,
    "local_address": "127.0.0.1",
    "local_port":1080,
    "password":"server_password",
    "timeout":300,
    "method":"aes-256-cfb",
    "fast_open": false,
    "workers": 1,
    "prefer_ipv6": false
}
```

Start client

```sh
sslocal -c /etc/shadowsocks/config.json -d start
```

```txt
$ sslocal --help
usage: sslocal [OPTION]...
A fast tunnel proxy that helps you bypass firewalls.

You can supply configurations via either config file or command line arguments.

Proxy options:
  -c CONFIG              path to config file
  -s SERVER_ADDR         server address
  -p SERVER_PORT         server port, default: 8388
  -b LOCAL_ADDR          local binding address, default: 127.0.0.1
  -l LOCAL_PORT          local port, default: 1080
  -k PASSWORD            password
  -m METHOD              encryption method, default: aes-256-cfb
  -t TIMEOUT             timeout in seconds, default: 300
  -a ONE_TIME_AUTH       one time auth
  --fast-open            use TCP_FASTOPEN, requires Linux 3.7+

General options:
  -h, --help             show this help message and exit
  -d start/stop/restart  daemon mode
  --pid-file PID_FILE    pid file for daemon mode
  --log-file LOG_FILE    log file for daemon mode
  --user USER            username to run as
  -v, -vv                verbose mode
  -q, -qq                quiet mode, only show warnings/errors
  --version              show version information

Online help: <https://github.com/shadowsocks/shadowsocks>
```

## Resources

### Tutorial

* [**YouTube - 哪種翻牆軟件更隱蔽？！聯通後台數據實測SS/SSR/V2Ray/Brook 翻牆APP！請耐心看完本教程，能讓你避免被請喝茶！**](https://www.youtube.com/watch?v=G-P8eyltc5E) - Protocols explaination
  * [Tutorial blog](https://telegra.ph/Happy-New-World-08-11)
* [YouTube - Shadowsocks零基礎上手/把手教你設置SSR.SS客戶端/附送大量免費SS節點（翻牆/科學上網/SS.SSR翻牆/SS.SSR免費節點）](https://youtu.be/Y_ToiGM266Y)
