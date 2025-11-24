# Miden Node Guide
Guide to Installation Miden Node

## Install Package

#### Install Dependencies

```
sudo apt install llvm cargo clang bindgen pkg-config libssl-dev libsqlite3-dev
```

#### Install rustc 

```
curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh
source $HOME/.cargo/env
```

```
rustc --version
```

#### Install miden node

```
cargo install miden-node --locked
```
