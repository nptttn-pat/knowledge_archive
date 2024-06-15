# Basic command-line
To find the ROS package

- ```rospack find roscpp```

To change directory to ROS package

- `roscd roscpp`

# Create your workspace
To create your ROS workspace
- `mkdir -p <workspace_name>/src`
- `cd <workspace_name>/`
- `catkin_make`

# Create your package
   - `cd src/`

Create package by using catkin_create_pkg

- `catkin_create_pkg <package_name> <dependency_1> <dependency_1>`

   <i>Example</i>
   - `catkin_create_pkg <package_name> rospy roscpp std_msgs`
