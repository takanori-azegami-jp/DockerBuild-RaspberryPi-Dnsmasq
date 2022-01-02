# DockerBuild-RaspberryPi-Dnsmasq
RaspberryPiにDockerでDnsmasqをたてる

## コンテナ起動
~~~powershell
PS C:\>  docker-compose up -d --build
~~~

## コンテナ接続
~~~powershell
#コンテナID取得
PS C:\>  docker ps 
#コンテナに接続
PS C:\>  docker exec -it コンテナID bash
~~~


## 参考
[DnsmasqをDockerで起動する](https://scribble.washo3.com/dnsmasq_on_docker.html)
