# Nexus-CLI-Node-Run-Manual


Windows & macOS

→ windows: Install WSL (Windows Subsystem for Linux) 

→ macOS: `run brew install git`

# Step 1: Update Ubuntu & install required packages

linux:
`sudo apt update && sudo apt upgrade -y`
`sudo apt install -y build-essential pkg-config libssl-dev protobuf-compiler`


# Step 2: Install Rust
`curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh -s -- -y
source "$HOME/.cargo/env"
exec "$SHELL"`

# Step 3: Verify Rust installation
`cargo --version`

# Step 4: Add RISC-V target for Rust
`rustup target add riscv32i-unknown-none-elf`

# Step 5: Install Nexus CLI
`curl https://cli.nexus.xyz/ | sh`


Nexus CLI Error & Fix

If you're facing a byte error while running Nexus CLI, try this fix:

`sudo fallocate -l 10G /swapfile && sudo chmod 600 /swapfile && sudo mkswap /swapfile && sudo swapon /swapfile && echo`



Twitter (x) 
https://x.com/KadyBit/status/1892219364176511432

follow for more updates
