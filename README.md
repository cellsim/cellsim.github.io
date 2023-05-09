# cellsim.github.io

## Installation

```
curl -fsSL https://cellsim.github.io/debian/gpg.key | gpg --dearmor | sudo tee /etc/apt/trusted.gpg.d/cellsim-apt-key.gpg > /dev/null
echo "deb https://cellsim.github.io/debian/buster buster main" | sudo tee /etc/apt/sources.list.d/cellsim.list
sudo apt update
sudo apt install cellsim
```

## Setup

See https://github.com/cellsim/multisend#simulation
