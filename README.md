# rinetd

```shell
wget https://github.com/chinayin/rinetd/archive/v0.62.tar.gz -O ./rinetd.tar.gz
tar -xvf rinetd.tar.gz && cd rinetd
mkdir /usr/man && make && make install
```

`/etc/rinetd.conf`
```shell
0.0.0.0 8282 xx.xx.xx.xx 8282
logfile /var/log/rinetd.log
```

```shell
echo "/usr/sbin/rinetd -c /etc/rinetd.conf" >> /etc/rc.local

chmod +x /etc/rc.d/rc.local
```

```shell
pkill rinetd
```
