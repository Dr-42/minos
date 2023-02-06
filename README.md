#MINOS

A mini os based https://os.phil-opp.com .

## Rustup

Install rustup in your working system

### Windows 
Download and use the rustup-init.exe from the rustup website
### MSYS2
Run in MINGW64 terminal
```
pacman -S git && pacman -S mingw-w64-x86_64-toolchain
curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh
```

Select x86_64-pc-windows-gnu as host triple. Choose the rest as default.
Add to .bashrc or .zshrc depending on shell
```
export PATH="/c/Users/<username>/.cargo/bin:$PATH"
```
### Linux
run 
```
curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh
```

Select defaults.

## Project config
In the projeect directory
```
rustup override set nightly
rustup component add rust-src
rustup component add llvm-tools-preview
cargo install bootimage
```

## Running
```
cargo run
```
