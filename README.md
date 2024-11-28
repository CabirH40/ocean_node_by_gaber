### 1. Install Docker (using sudo)
To install Docker, run the following command:

```bash
sudo bash -c "$(curl -s https://get.docker.com)"
### 2.Install Ocean Node
sudo mkdir -p /home/$USER/ocean && cd /home/$USER/ocean
sudo bash -c "$(curl -s https://raw.githubusercontent.com/oceanprotocol/ocean-node/main/scripts/ocean-node-quickstart.sh)"
