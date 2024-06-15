REF: [Install ROS noetic on Ubuntu](http://wiki.ros.org/noetic/Installation/Ubuntu)

# ROS installation
Add apt source list for ROS repository
```
sudo sh -c 'echo "deb http://packages.ros.org/ros/ubuntu $(lsb_release -sc) main" > /etc/apt/sources.list.d/ros-latest.list'
```

Install curl
```
sudo apt install curl
```

Get ROS installation key from server
```
curl -s https://raw.githubusercontent.com/ros/rosdistro/master/ros.asc | sudo apt-key add -
```

Update apt server
```
sudo apt update
```

Install ROS noetic (with full desktop apps)
```
sudo apt install ros-noetic-desktop-full
```

Add setup file to .bashrc (Run everytime when open terminal)
```
echo "source /opt/ros/noetic/setup.bash" >> ~/.bashrc
```

Force terminal to read .bashrc
```
source ~/.bashrc
```

Install another depencies for ROS noetic
```
sudo apt install python3-rosdep python3-rosinstall python3-rosinstall-generator python3-wstool build-essential
```

Initialize ROS depencies package
```
sudo rosdep init
```

Update the ROS depencies package
```
rosdep update
```

# Test ROS installation
Running ROS master with roscore
```
roscore
```