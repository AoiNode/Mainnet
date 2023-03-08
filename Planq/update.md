#Update PlanQ cosmovisor version

````sudo systemctl stop planqd````

```wget https://github.com/planq-network/planq/releases/download/v1.0.5/planq_1.0.5_Linux_x86_64.tar.gz && tar -C ~/.planqd/cosmovisor/current -xzf planq_1.0.5_Linux_x86_64.tar.gz```
*Change the link and the name to the new version

```sudo systemctl start planqd```
