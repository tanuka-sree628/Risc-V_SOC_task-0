# 🖥️ Risc-V_ Reference_SOC_ tapeout program_task-0
This repository dwelves with my task completion on the program "India RISC-V Chip Tapeout". Hereby completing my first task of installing the tools needed for the program.
#📅 **WEEK 0- TASK 0 SETUP AND TOOLS**
## System requirements
Below are the system requirements for the tools to be installed
-Operating system--Ubuntu 24.03 (latest version)
-RAM--8GB
-Disk Space--50GB
-CPU--4 core
-Tools/softwares--yosys,iverilog,GTKWave
# **TOOLS INSTALLED**
-Yosys
-iverilog
-GTKWave
These are installed in Ubuntu 24.03 using Orcale Virtual Machine 7.2.2
# TOOLS CHECK
**YOSYS**
```bash
$ sudo apt-get update
$ git clone https://github.com/YosysHQ/yosys.git
$ cd yosys
$ sudo apt install make               # If make is not installed
$ sudo apt-get install build-essential clang bison flex \
    libreadline-dev gawk tcl-dev libffi-dev git \
    graphviz xdot pkg-config python3 libboost-system-dev \
    libboost-python-dev libboost-filesystem-dev zlib1g-dev
$ make config-gcc
$ git submodule update --init --recursive
$ make 
$ sudo make install

