# streaming

클라우드를 사용하지 않을 경우 아래 파일을 수정하여 고정ip 를 셋팅. 랜카드가 eth0 가 아닐 수도 있음
/etc/network/interfaces

auto eth0

iface eth0 inet static

  address xxx.xxx.xxx.xxx
  
  netmask 255.255.255.0
  
  gateway xxx.xxx.xxx.xxx
  

/etc/resolv.conf

nameserver xxx <- this would be automatically added.


/etc/init.d/networking restart


cd ~

apt-get install git

git clone https://github.com/candicom/streaming.git

위 명령어를 통해 필요 파일 다운로드.
