# Basic command-line
To find the ROS package
```
rospack find roscpp
```

To change directory to ROS package
```
roscd roscpp
```

# Create your workspace
To create your ROS workspace
```
mkdir -p <workspace_name>/src
```

Change directory to your workspace
```
cd <workspace_name>/
```

Make your workspace
```
catkin_make
```

# Create your package
Change directory to src
```
cd src/
```

Create package by using catkin_create_pkg
```
catkin_create_pkg <package_name> <dependency_1> <dependency_2>
```

   <i>Example</i>
   ```
   catkin_create_pkg <package_name> rospy roscpp std_msgs
   ```