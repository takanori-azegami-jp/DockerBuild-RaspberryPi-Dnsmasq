# DockerBuild-RaspberryPi-Dnsmasq
内部向けのDNSサーバ構築する<br>
RaspberryPi(32bit)にDockerでDnsmasqを構築

## コンテナ起動
docker-compose.ymlを配置したフォルダに移動して実行
~~~
$ docker-compose up -d --build
~~~

## 名前解決は/etc/hostsで行う
~~~
$ vi /etc/hosts
~~~

## DNSに問い合わせ
~~~
digの場合
$ dig @[DNSホストのIP] ドメイン名
nslookupの場合
$ nelookup ドメイン名　[DNSホストのIP]
~~~

## 参考
[DnsmasqをDockerで起動する](https://scribble.washo3.com/dnsmasq_on_docker.html)

RaspberryPi(arm32bit)環境でビルドされた下記Dockerイメージを使用<br>
[Docker Hub：jasjeev4/rpi-dnsmasq](https://hub.docker.com/r/jasjeev4/rpi-dnsmasq)
