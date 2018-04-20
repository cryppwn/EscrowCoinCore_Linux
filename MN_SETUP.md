# Masternode Setup
This guide will walk you through setting up an ESCO (Escrow-Coin) Masternode on an Ubuntu VPS. The goal of this method is to simplify the overall installation while simulatenously allowing multiple MNs to run on the same VPS. 

### Pre-Requisites
- Ubuntu 16.04 Virtual Private Server (VPS)
- SSH configuration for accessing server (putty, or terminal apps)

### VPS Initial Setup
This section will get you started for your initial setup of the VPS for best functionality.

SSH into your VPS and run the following commands:
```
sudo apt-get install git 
git clone https://github.com/cryppwn/EscrowCoinCore_Linux.git
```

This will create an EscrowCoinCore_Linux directory. Once the download is complete, go into the scripts directory and run some initial configuration scripts. Feel free to review them yourself to understand what they are doing.
```
cd EscrowCoinCore_Linux/scripts
./update_ubuntu.sh
./install_docker.sh
```
These commands may take some time, so please be patient. The `install_docker` script requires manual confirmation of the Docker Engine's apt fingerprint.

**TODO** ADD SCREENSHOT
