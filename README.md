# Miden Node Guide
Guide to Installation Miden Node

#### Specification

Minimum Specifiaction :

- 4 core CPU
- 8 gb ram

## Install Package

#### Install Dependencies

```bash
sudo apt install llvm cargo clang bindgen pkg-config libssl-dev libsqlite3-dev
```

#### Install rustc 

```bash
curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh
source $HOME/.cargo/env
```

```bash
rustc --version
```

#### Install miden node

```
cargo install miden-node --locked
```

#### Create Miden Directory

```bash
mkdir miden
cd miden
```

#### Bootstraping
```bash
miden-node bundled bootstrap \
  --data-directory data \
  --accounts-directory accounts
```

#### Run node

Run inside screen

```bash
screen -S miden
```

Make sure in miden directory

```bash
cd ~/miden
```

run miden node

```bash
miden-node bundled start \
  --data-directory data \
  --rpc.url http://0.0.0.0:57291
```



