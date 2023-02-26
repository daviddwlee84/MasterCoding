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
    * Android
      * BifrostV
      * [Releases · 2dust/v2rayNG](https://github.com/2dust/v2rayNG/releases)
    * [V2rayU](https://github.com/yanue/V2rayU) - macOS

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

* [free resources](https://flywind.ml/free-ss)
* https://github.com/the0demiurge/ShadowSocksShare

Heroku

* [mrluanma/shadowsocks-heroku](https://github.com/mrluanma/shadowsocks-heroku)
* [shadowsocks/shadowsocks-manager: A shadowsocks manager tool for multi user and traffic control.](https://github.com/shadowsocks/shadowsocks-manager)
* Auto Deploy
  * [teddysun/shadowsocks_install at master](https://github.com/teddysun/shadowsocks_install/tree/master)
* Deploy by one button
  * [onplus/shadowsocks-heroku: 一键部署 Free Shadowsocks-Heroku](https://github.com/onplus/shadowsocks-heroku)
  * [shadowsocks-websocket-python/README.md at deploy · onplus/shadowsocks-websocket-python](https://github.com/onplus/shadowsocks-websocket-python/blob/deploy/README.md)

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

### Deploy on Heroku

> This is not compatible with the normal SS client

* Use other's Heroku Template: [Click here](https://heroku.com/deploy?template=https://github.com/onplus/shadowsocks-heroku/tree/re)

> you will get `app-name.herokuapp.com` as link to your server

Requirement

* Client: [release](https://github.com/onplus/shadowsocks-heroku/releases) ([backup](https://github.com/onplus/archive/tree/master/tool))
  * Mac
    1. Modify the default configure in `config.json` (server, password, method)
    2. Execute the client: `./ss-h`
* Chrome Extension: [SwitchyOmega](https://github.com/FelisCatus/SwitchyOmega) - [release](https://github.com/FelisCatus/SwitchyOmega/releases), [Chrome Web Store](https://chrome.google.com/webstore/detail/proxy-switchyomega/padekgcemlokbadohgkifijomclgjgif)
  1. Add a new profile
  2. Set proxy servers
     * Protocol: SOCKS5
     * Server: 127.0.0.1
     * Port: 1080

## Resources

https://github.com/cnlh/nps

https://bbs.pku.edu.cn/v2/post-read.php?bid=35&threadid=16264150

[SS/SSR - 这本书能让你连接互联网 Ⅱ](https://hoodiearon.github.io/fq-book/#/proxy/ss-ssr)

v2ray
[2dust/v2rayN](https://github.com/2dust/v2rayN)
[2dust/v2rayNG](https://github.com/2dust/v2rayNG)
[yanue/V2rayU: V2rayU,基于v2ray核心的mac版客户端,用于科学上网,使用swift4.2编写,支持vmess,shadowsocks,socks5等服务协议,支持订阅, 支持二维码,剪贴板导入,手动配置,二维码分享等](https://github.com/yanue/V2rayU)
[onplus/v2hero: All Free . Deploy V2Ray to Heroku . v2ray学习参考](https://github.com/onplus/v2hero)

[EtherDream/jsproxy: 一个基于浏览器端 JS 实现的在线代理](https://github.com/EtherDream/jsproxy)

[hmgle/graftcp: A flexible tool for redirecting a given program's TCP traffic to SOCKS5 or HTTP proxy.](https://github.com/hmgle/graftcp)

### Mirror

* [Tuna](https://mirror.tuna.tsinghua.edu.cn)
  * [pypi](https://mirror.tuna.tsinghua.edu.cn/help/pypi/)
    * `pip install -i https://pypi.tuna.tsinghua.edu.cn/simple some-package`
  * [raspbian](https://mirror.tuna.tsinghua.edu.cn/help/raspbian/)
  * [ubuntu](https://mirror.tuna.tsinghua.edu.cn/help/ubuntu/)

### Tutorial

* [**YouTube - 哪種翻牆軟件更隱蔽？！聯通後台數據實測SS/SSR/V2Ray/Brook 翻牆APP！請耐心看完本教程，能讓你避免被請喝茶！**](https://www.youtube.com/watch?v=G-P8eyltc5E) - Protocols explaination
  * [Tutorial blog](https://telegra.ph/Happy-New-World-08-11)
* [YouTube - Shadowsocks零基礎上手/把手教你設置SSR.SS客戶端/附送大量免費SS節點（翻牆/科學上網/SS.SSR翻牆/SS.SSR免費節點）](https://youtu.be/Y_ToiGM266Y)
* [YouTube - 2019科學上網翻牆誰最快? SS/SSR/V2Ray/WireGuard在谷歌雲搬瓦工上速度對比（科學上網翻牆速度大比拼）](https://www.youtube.com/watch?v=9UkVDoZpOYE)
