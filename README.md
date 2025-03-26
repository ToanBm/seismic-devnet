# Seismic Devnet Create and Interact with First contract
# Hardware
The minimum hardware requirements for running an Initia node are:
```bash
CPU: 2 cores
Memory: 4GB RAM
```
# Deploy an encrypted contract
## Step 1
Update all the packages
```
sudo apt update && sudo apt install git -y && sudo apt install build-essential -y
```
Install Rust
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
## Step2: 

install `jq`

```
sudo apt install jq
```

## Step 3
Install sfoundryup
```bash
curl -L \
     -H "Accept: application/vnd.github.v3.raw" \
     "https://api.github.com/repos/SeismicSystems/seismic-foundry/contents/sfoundryup/install?ref=seismic" | bash
```
```bash
source /root/.bashrc
```
```bash
sfoundryup
```
## step 4
clone the repository
```bash
git clone --recurse-submodules https://github.com/SeismicSystems/try-devnet.git && cd try-devnet/packages/contract/
```
## Step 5 
Deploy contract
```
bash script/deploy.sh
```

go to https://faucet-2.seismicdev.net/ and then enter the address show on image to get token.
wait 15-30 seconds then hit enter and enjoys the rest. 
you have done when you see 
# Interact with deploy contract
## step 1
install **bun**

```
cd
curl -fsSL https://bun.sh/install | bash
```
## step 2 
run 
```bash
cd try-devnet/packages/cli/
bun install
```
## step 3

run 

```bash
bash script/transact.sh
```
you will see this again. inside
- step1: hit enter
- step2: 

![alt text](./images/image4.png)

go to https://faucet-2.seismicdev.net/ and then enter the address show on image to get token.

![alt text](./images/image5.png)

wait 15-30 seconds then hit enter and enjoys the rest. 

you have done when you see 

![alt text](./images/image7.png)

when you come to this place. You are doing the good job.


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

Take the screenshot both 2 Deploy and interact an encrypted contract.  Then post it on it X. https://x.com/leiz95/status/1904779356053946544

