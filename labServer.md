# labServer

实验室服务器配置相关

> Ubuntu 18.04 LTS

LAN fixed IP: 192.168.1.110

## Initial

### SSH configure:

- user ruiyun
- port 222
- Connect by `ssh -p 222 ruiyun@ruiyun.local` in LAN

Linux:
You can add public key in server:

> ssh-copy-id ruiyun@ruiyun.local -p 222

Set an `alias` like `ryssh`

> ssh ruiyun@ruiyun.local -p 222

### Server configure

国内源自己搜,source list set:

> /etc/apt/sources.list

host 更改:

> /etc/hosts

添加记录:

> 192.168.1.110 ruiyun.org

### LAMP 服务配置

Learn from this link: [LAMP-stack-digital-ocean](https://www.digitalocean.com/community/tutorials/how-to-install-linux-apache-mysql-php-lamp-stack-ubuntu-18-04)

### PHPMyAdmin 方便观看 sql

1. [digital-ocean](https://www.digitalocean.com/community/tutorials/how-to-install-and-secure-phpmyadmin-on-ubuntu-18-04)

2. ATTENTION: 在配置的时候必须用`space`或者`tab`来选择 apache2

3. 建立 softLink:
   > sudo ln -s /usr/share/phpmyadmin /var/www/ruiyun.org/phpmyadmin
4. 配置安全账户密码 账号为: ruiyun pwd: `+=`123

### Redis 配置

[digital-ocean](https://www.digitalocean.com/community/tutorials/how-to-install-and-secure-redis-on-ubuntu-18-04)

## copy between client and server

[ReferLink-SCP](https://unix.stackexchange.com/questions/106480/how-to-copy-files-from-one-machine-to-another-using-ssh)

example:

> scp -P 222 /path/to/file USERNAME@IP:/path/to/destination

**More by update in the future.**
