# Learn To Be A Robot Development Engineer

My plan is to learn the applications of C++ and Python on Linux systems, and integrate them for practical use via ROS 2.

In the previous repositories, I have learned about the basic Linux system commands.

But if you want to use ROS2, you need to install Ubuntu 24.04 LTS as the software with VMware.

You can download at https://mirrors.tuna.tsinghua.edu.cn/ubuntu-releases/24.04.4/

## Install The Basic Tools 

You need to download and install some tools and softwares before you start working.

### Install VMware tools

1. Open Terminal

2. Input these commands

```bash
sudo apt update
sudo apt install open-vm-tools open-vm-tools-desktop
sudo reboot
```

### Update Ubuntu

1. Open Terminal

2. Input these commands

```bash
sudo apt update
sudo apt upgrade
```

### Install Basic Tools

1. Open Terminal

2. Input these commands 

```bash
sudo apt install build-essential cmake git curl wget vim tree htop net-tools unzip
```

It includes gcc  g++  make  cmake  git

### Install VS Code

1. Open Terminal

2. Input these commands

```bash
sudo snap install code --classic
```

### Install C/C++ CMake GBD

1. Open Terminal

2. Input these commands

```bash
sudo apt install -y build-essential
sudo apt install -y cmake
sudo apt install -y gdb
```

### Install Python pip

1. Open Terminal

2. Input these commands

```bash
sudo apt install -y python3-pip
sudo apt install -y python3-venv

sudo apt install -y \
python3-numpy \
python3-matplotlib \
python3-pandas \
python3-scipy

sudo apt install -y python3-opencv
```

### Install ROS2

1. Open Terminal

2. Input these commands

```bash
sudo apt install -y software-properties-common curl gnupg2 lsb-release

sudo add-apt-repository universe

sudo curl -sSL https://raw.githubusercontent.com/ros/rosdistro/master/ros.key \
-o /usr/share/keyrings/ros-archive-keyring.gpg

sudo apt update

sudo apt install -y ros-jazzy-desktop

echo "source /opt/ros/jazzy/setup.bash" >> ~/.bashrc

source ~/.bashrc

sudo apt install -y \
python3-colcon-common-extensions \
python3-rosdep \
python3-vcstool \
python3-argcomplete

sudo rosdep init

rosdep update

mkdir -p ~/ros2_ws/src

cd ~/ros2_ws

colcon build

echo "source ~/ros2_ws/install/setup.bash" >> ~/.bashrc

source ~/.bashrc
```

### Install Git

1. Open Terminal

2. Input these commands

```bash
sudo apt install -y git
git config --global user.name "your-GitHub-user-name"
git config --global user.email "your-email"
git config --list
```

### Test

You can test if the softwares are installed

Input these commands

```bash
gcc --version
g++ --version
cmake --version
python3 --version
pip3 --version
git --version
ros2 --help
```

## Summary
