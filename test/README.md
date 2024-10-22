curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh

. "$HOME/.cargo/env"

cd .. 

time ./target/release/lust test/fib.lua

sudo apt install lua5.3 luajit

lua test/fib.lua

luajit  test/fib.lua
