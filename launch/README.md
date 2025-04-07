# Launch Files

This directory contains the ROS2 launch files used to run the FAST-LIO SLAM system.

## Files

- **mapping.launch.py**: Main launch file for FAST-LIO
- **msg_MID360_launch.py**: Launch file for the Livox Mid-360 driver

## Usage

To run the complete SLAM system, execute these launch files in separate terminals:

```bash
# Terminal 1: Start the Livox driver
ros2 launch livox_ros_driver2 msg_MID360_launch.py

# Terminal 2: Start FAST-LIO
ros2 launch fast_lio mapping.launch.py config_file:=mid360.yaml
