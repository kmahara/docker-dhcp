## 概要

以下の Dockerfikle をベースに改造したもの。  
https://github.com/container-images/dhcp-server.git

変更点:
* オリジナル版ではホストの以下のディレクトリをマウントする仕様だが、マウントしないよう変更。  
  * /etc/dhcp
  * /var/lib/dhcpd

