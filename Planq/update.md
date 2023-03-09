Update PlanQ

[Cosmovisor]  
```
sudo systemctl stop planqd

wget https://github.com/planq-network/planq/releases/download/v1.0.5/planq_1.0.5_Linux_x86_64.tar.gz && tar -C ~/.planqd/cosmovisor/current -xzf planq_1.0.5_Linux_x86_64.tar.gz

planqd version
#commit: f6bf105a30a72f2e55b42792136fc72fa519ca9c
#version: 1.0.5

systemctl restart planqd && journalctl -fu planqd -o cat```
```
[Not Cosmovisor]
```
sudo systemctl stop planqd
cd $HOME
rm -rf planq
git clone https://github.com/planq-network/planq
cd planq
git pull 
git checkout v1.0.5
make install

planqd version
#commit: f6bf105a30a72f2e55b42792136fc72fa519ca9c
#version: 1.0.5

systemctl restart planqd && journalctl -fu planqd -o cat
```



Change the link and name to the specific version
