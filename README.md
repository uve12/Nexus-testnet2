# Nexus-testnet2
Full guide to Nexus testnet2 Cli node.

Unlock the Power of Verifiable Computation

Site : [Nexus](https://nexus.xyz/) | X : [NexusLabs](https://x.com/NexusLabsHQ) | Docs : [Nexus docs](https://docs.nexus.xyz/)


# Join Crypto Console Community

Join TG : [Crypto Console Telegram](https://t.me/cryptoconsol) 

Follow X : [Crypto Console Twitter](https://www.x.com/cryptoconsol) 

Subscribe : [Crypto Console Youtube](https://www.youtube.com/@cryptoconsole)

## Hardware requirements:

| **Hardware** | **Minimum Requirement** |
|--------------|-------------------------|
| **CPU**      | 4 Cores                 |
| **RAM**      | 6 GB                    | 
| **Disk**     | 50  GB  SSD             |


# VPS Options

VPS 1 is enough for Nexus Prover


💻 Contabo VPS Deals 🚀 Buy with Credit Card/Paypal/Crypto Credit card : 

 

| **VPS** | **Direct Link**                      |
|---------|--------------------------------------|
| VPS 1   | [Contabo VPS 1](https://www.jdoqocy.com/click-101278318-15692486) |
| VPS 2   | [Contabo VPS 2](https://www.anrdoezrs.net/click-101278318-13796472) |
| VPS 3   | [Contabo VPS 3](https://www.dpbolvw.net/click-101278318-13796474) |
| VPS 4   | [Contabo VPS 4](https://www.anrdoezrs.net/click-101278318-13796476) |


💡 **Get started with the perfect VPS for your needs!** 🚀


---


Create Account

Visit the Nexus App: https://app.nexus.xyz and create an account. A wallet will be automatically created for you.

**Link to Nexus Account**

- Create an account at app.nexus.xyz.

- Follow the account linking instructions.

- Your contributions will earn NEX Points.

- Track your progress on the leaderboard.

- Manage all your nodes in one place.

### Install dependencies
```
sudo apt update && sudo apt upgrade
sudo apt install build-essential pkg-config libssl-dev git-all curl screen unzip
```

### Install Protobuf

The protobuf Installation steps might be different from shown in the video. No issues, Just copy and paste step by step.

```
sudo apt remove --purge -y protobuf-compiler
rm -rf $HOME/.local/bin/protoc
rm -rf $HOME/.local/include/google
```
```
PROTOC_VERSION=25.3
wget https://github.com/protocolbuffers/protobuf/releases/download/v${PROTOC_VERSION}/protoc-${PROTOC_VERSION}-linux-x86_64.zip -O protoc.zip

```
```
unzip -o protoc.zip -d $HOME/.local
rm protoc.zip  # Cleanup the downloaded file

```
```
echo 'export PATH="$HOME/.local/bin:$PATH"' >> ~/.bashrc
echo 'export PROTOC="$HOME/.local/bin/protoc"' >> ~/.bashrc
source ~/.bashrc

```

```
protoc --version
```


Result should be **libprotoc 25.3**


### Install Rust
```
curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh
```
```
source $HOME/.cargo/env
```
```
rustup target add riscv32i-unknown-none-elf
```

### Open Screen and Start Node
```
screen -S nexus
```
```
curl https://cli.nexus.xyz/ | sh
```
---

**Follow** : https://x.com/cryptoconsol
