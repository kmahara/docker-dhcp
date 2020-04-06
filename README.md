## 概要

以下の Dockerfikle をベースに改造したもの。  
https://github.com/container-images/dhcp-server.git

変更点:
* オリジナル版ではホストの以下のディレクトリをマウントする仕様だが、マウントしないよう変更。  
  * /etc/dhcp
  * /var/lib/dhcpd

## セットアップ手順

```
mkdir /docker
cd /docker
git clone https://github.com/kmahara/docker-dhcp.git
mv docker-dhcp dhcp
```

設定ファイルを編集。

```
vi etc/dhcpd.conf
```

起動

```
docker-compose up -d
```
