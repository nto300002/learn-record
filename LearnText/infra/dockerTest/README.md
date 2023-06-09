https://sagantaf.hatenablog.com/entry/2019/12/18/234553
docker network --help
docker network ls
## bridgeネットワークの詳細
docker network inspect bridge
ifconfig docker0
ip link show docker0

## コンテナを起動してホストのネットワーク構成の変化を確認する
sudo docker run -d --name test1 alpine sleep 6000
ip link
brctl show
ifconfig veth3d3f000
