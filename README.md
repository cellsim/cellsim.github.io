# cellsim.github.io

## Installation

```
curl -fsSL https://cellsim.github.io/debian/gpg.key | gpg --dearmor | sudo tee /etc/apt/trusted.gpg.d/cellsim-apt-key.gpg > /dev/null
echo "deb https://cellsim.github.io/debian/cellsim cellsim main" | sudo tee /etc/apt/sources.list.d/cellsim.list
sudo apt update
sudo apt install cellsim
```

## Setup

See [multisend](https://github.com/cellsim/multisend#simulation)

```
$ sudo apt install cellsim
Reading package lists... Done
Building dependency tree... Done
Reading state information... Done
The following NEW packages will be installed:
  cellsim
0 upgraded, 1 newly installed, 0 to remove and 4 not upgraded.
Need to get 2,164 kB of archives.
After this operation, 0 B of additional disk space will be used.
Get:1 https://cellsim.github.io/debian/cellsim cellsim/main arm64 cellsim arm64 1.0 [2,164 kB]
Fetched 2,164 kB in 1s (2,247 kB/s)  
Selecting previously unselected package cellsim.
(Reading database ... 131664 files and directories currently installed.)
Preparing to unpack .../archives/cellsim_1.0_arm64.deb ...
Unpacking cellsim (1.0) ...
Setting up cellsim (1.0) ...
Init the setup: "/opt/cellsim/cellsim-setup.sh [ingress] [egress]"
To run cellsim emulator:
nohup sudo cellsim [uplink_trace] [downlink_trace] [loss] [ingress] [egress] > /tmp/cellsim-stdout 2>/tmp/cellsim-stderr
Preinstalled trace files can be found at "/opt/cellsim/traces"
To stop cellsim emulator:
killall cellsim
```
