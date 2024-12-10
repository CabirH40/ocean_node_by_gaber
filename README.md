# ocean_node_by_gaber
🖥Hardware Requirements:
➡️CPU: 1vcpu
➡️Memory: 2 GB ram
➡️Storage: 4 GB storage
➡️OS: we recommend using the latest LTS version of Ubuntu or the latest macOS. However, the nodes should also work on other operating systems including Windows.

### 1. Install Docker (using sudo)

don't copy all just step by step 
```bash
sudo bash -c "$(curl -s https://get.docker.com)"
sudo mkdir -p /home/$USER/ocean 
cd /home/$USER/ocean
sudo bash -c "$(curl -s https://raw.githubusercontent.com/oceanprotocol/ocean-node/main/scripts/ocean-node-quickstart.sh)"
### When prompted:

Do you have your private key for running the Ocean Node [ y/n ]: Type N if you don’t have a private key.
Do you want me to create a private key for you [ y/n ]: Type Y to generate a new private key.
Make sure to save the private key securely after it’s generated.
enter the evm adress 
Provide the HTTP_API_PORT value or accept the default (press Enter) [8000]:ENTER
Provide the P2P_ipV4BindTcpPort or accept the default (press Enter) [9000]:ENTER
Provide the P2P_ipV4BindWsPort or accept the default (press Enter) [9001]:ENTER
Provide the P2P_ipV6BindTcpPort or accept the default (press Enter) [9002]:ENTER
Provide the P2P_ipV6BindWsPort or accept the default (press Enter) [9003]:ENTER
Provide the public IPv4 address or FQDN where this node will be accessible: your vps global ip and ENTER

### Run code:
sudo docker compose up -d
### logs
sudo docker compose logs -f



###Check Ocean Node Status:
http://yourserverIp:8000/dashboard/
