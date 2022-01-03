# DockerBuild-RaspberryPi-Dnsmasq
内部向けのDNSサーバ構築する
RaspberryPiRaspberryPi(32bit)にDockerでDnsmasqをたてる

## コンテナ起動
docker-compose.ymlを配置したフォルダに移動して実行
~~~powershell
PS C:\>  docker-compose up -d --build
~~~

## DNSに問い合わせ
~~~console
  $ dig hoge1.example.com
~~~

## 参考
[DnsmasqをDockerで起動する](https://scribble.washo3.com/dnsmasq_on_docker.html)
