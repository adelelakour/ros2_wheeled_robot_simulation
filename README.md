# ROS 2 Wheeled Robot + 2-DOF Arm (Gazebo Sim + RViz)

A ROS 2 project that spawns a wheeled robot with a simple 2-joint arm from URDF/Xacro, simulates it in Gazebo Sim (Ignition / gz-sim), and visualizes the TF and robot model in RViz. Joint position commands and joint states are bridged between ROS 2 and Gazebo using `ros_gz_bridge`.

## Packages
- `my_robot_description` — URDF/Xacro robot model
- `my_robot_bringup` — launch files, world, bridge config (`gazebo_bridge.yaml`)

## Requirements
- ROS 2 (Humble or newer recommended)
- Gazebo Sim (Ignition / gz-sim)
- `ros_gz_sim`
- `ros_gz_bridge`

## Build
```bash
colcon build --symlink-install
source install/setup.bash

## Run
- ros2 launch my_robot_bringup my_robot_gazebo.launch.xml


