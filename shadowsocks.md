# Shadowsocks
## Install
```
wget --no-check-certificate -O shadowsocks-go.sh https://raw.githubusercontent.com/teddysun/shadowsocks_install/master/shadowsocks-go.sh
chmod +x shadowsocks-go.sh
./shadowsocks-go.sh 2>&1 | tee shadowsocks-go.log
```

## Install Success
```
Congratulations, Shadowsocks-go install completed!
Your Server IP:your_server_ip
Your Server Port:your_server_port
Your Password:your_password
Your Local Port:1080
Your Encryption Method:aes-256-cfb

Welcome to visit:https://teddysun.com/392.html
Enjoy it!
```
## Uninstall

```
./shadowsocks-go.sh uninstall
```

## Command
```
start:    /etc/init.d/shadowsocks start
stop:     /etc/init.d/shadowsocks stop
restart:  /etc/init.d/shadowsocks restart
status:   /etc/init.d/shadowsocks status
```
## Config
path:
```
/etc/shadowsocks/config.json
```
config:
```
{
    "port_password":{
         "8989":"password0",
         "9001":"password1",
         "9002":"password2",
         "9003":"password3",
         "9004":"password4"
    },
    "method":"aes-256-cfb",
    "timeout":600
}
```
