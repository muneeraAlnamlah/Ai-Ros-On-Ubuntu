## Install Ros On Ubuntu 

Installation
Configure your Ubuntu repositories
Configure your Ubuntu repositories to allow "restricted," "universe," and "multiverse." You can follow the Ubuntu guide for instructions on doing this.
 
Setup your sources.list
Setup your computer to accept software from packages.ros.org.

sudo sh -c 'echo "deb http://packages.ros.org/ros/ubuntu $(lsb_release -sc) main" > /etc/apt/sources.list.d/ros-latest.list'
 
Set up your key
sudo apt install curl # if you haven't already installed curl
 
curl -s https://raw.githubusercontent.com/ros/rosdistro/master/ros.asc | sudo apt-key add -

Installation
First, make sure your Debian package index is up-to-date:

sudo apt update
 
sudo apt install ros-noetic-desktop-full
 
Environment setup
source /opt/ros/noetic/setup.bash
 
echo "source /opt/ros/noetic/setup.bash" >> ~/.bashrc
 
Dependencies for building packages
sudo apt install python3-rosdep python3-rosinstall python3-rosinstall-generator python3-wstool build-essential
 
sudo apt install python3-rosdep
 
With the following, you can initialize rosdep:

sudo rosdep init
 
rosdep updat
 
