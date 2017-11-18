# docker-shadowsocks


Build a tiny docker image (compressed ~ 16MB) for shadowsocks based on [alpine](https://alpinelinux.org/)
linux. The versions of this dockerfile follows shadowsocks [releases](https://github.com/shadowsocks/shadowsocks/releases).


## Usage:

Pull the latest version from [docker hub](https://hub.docker.com/r/hzyuange/shadowsocks/):

```
docker pull hzyuange/shadowsocks
```

run it with command

```
docker run -d -p 8388:8388 --name shadowsocks hzyuange/shadowsocks -s 0.0.0.0 -p 8388 -m aes-256-cfb -k ${your_password}
```
