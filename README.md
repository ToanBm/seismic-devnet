# Seismic Devnet Create and Interact with First contract
### Hardware
The minimum hardware requirements for running an Initia node are:
```bash
CPU: 2 cores
Memory: 4GB RAM
```
## Step 1: Deploy an encrypted contract
### Update all the packages
```
sudo apt update && sudo apt install git -y && sudo apt install build-essential -y && sudo apt install unzip -y

```
### Install Rust
```
curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh -s -- -y
```
```
source $HOME/.cargo/env
```
- Check version
```
rustc --version
cargo --version
```
### Install jq
```
sudo apt install jq
```
### Install sfoundryup
```bash
curl -L \
     -H "Accept: application/vnd.github.v3.raw" \
     "https://api.github.com/repos/SeismicSystems/seismic-foundry/contents/sfoundryup/install?ref=seismic" | bash
```
```
source /root/.bashrc
```
### Run sfoundryup
```
sfoundryup
```
#### takes between 5m to 60m, and stalling for a while at 98% normal
### Clone the repository
```bash
git clone --recurse-submodules https://github.com/SeismicSystems/try-devnet.git && cd try-devnet/packages/contract/
```
### Deploy contract
```
bash script/deploy.sh
```
### When you see:
```
Step 2: Funding wallet
Please visit: https://faucet-2.seismicdev.net/
Enter this address: YOUR-WALLET-ADDRESS
Press Enter when done...
```
## Please faucet, check balance and ENTER to continue!
### Faucet
[Faucet](https://faucet-2.seismicdev.net/)
### Check balance on Explorer
[Explorer](https://explorer-2.seismicdev.net/)

##  Step 2: Interact with deploy contract
### Install Bun
```
cd
curl -fsSL https://bun.sh/install | bash
```
```
source /root/.bashrc
```
### Install node dependencies
```bash
cd try-devnet/packages/cli/
bun install
```
### Send transactions
```
bash script/transact.sh
```

### When you see:
```
Step 2: Funding wallet
Please visit: https://faucet-2.seismicdev.net/
Enter this address: YOUR-WALLET-ADDRESS
Press Enter when done...
```
## Please faucet, check balance and ENTER to continue!

### Take the screenshot both 2 Deploy and interact an encrypted contract. Then post it on it X. https://x.com/buiminhtoan1985/status/1904913621878190521

##   Done!

# Additional links Seismic Devnet:
```
Network Name: Seismic devnet
Currency Symbol: ETH
Chain ID: 5124
RPC URL (HTTP): https://node-2.seismicdev.net/rpc
RPC URL (WebSocket): wss://node-2.seismicdev.net/ws
Explorer: https://explorer-2.seismicdev.net
Faucet: https://faucet-2.seismicdev.net
Starter Repo: https://github.com/SeismicSystems/seismic-starter
```



