- [Install ROS noetic on Ubuntu](http://wiki.ros.org/noetic/Installation/Ubuntu)

# ROS installation
- `sudo sh -c 'echo "deb http://packages.ros.org/ros/ubuntu $(lsb_release -sc) main" > /etc/apt/sources.list.d/ros-latest.list'`
- `sudo apt install curl`
- `curl -s https://raw.githubusercontent.com/ros/rosdistro/master/ros.asc | sudo apt-key add -`
- `sudo apt update`
- `sudo apt install ros-noetic-desktop-full`
- `echo "source /opt/ros/noetic/setup.bash" >> ~/.bashrc`
- `source ~/.bashrc`
- `sudo apt install python3-rosdep python3-rosinstall python3-rosinstall-generator python3-wstool build-essential`
- `sudo rosdep init`
- `rosdep update`

# Test ROS installation
- `roscore`