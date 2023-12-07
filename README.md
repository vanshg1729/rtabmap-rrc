# RtabMap with RRC P3DX
This repo contains the launch and config files to make RtabMap run with RRC setup on a P3DX with RealSenseD455.

## Documentation
- All RtabMap documentation can be found on it's ros wiki page: [rtabmap_ros wiki](https://wiki.ros.org/rtabmap_ros/noetic_and_newer)

## Installation
To install RtabMap, follow the instructions on the official repo: [rtabmap_ros](https://github.com/introlab/rtabmap_ros)

## Running on RRC rosbag
There is an associated launch file for RRC hardware lab rosbag under `launch` folder, just download the [RRC rosbag]() 

### Visual Odometry (RGBD) Node
To try Rtabmap using visual odometry, simply run the following:
```
# In one terminal:
roslaunch rtabmap_launch visual_odom_p3dx.launch

# In another terminal:
rosbag play --clock <rrc_bag>.bag
```

### Wheel Odometry Node
```
# In one terminal
roslaunch rtabmap_launch wheel_odom_p3dx.launch

# In another terminal
rosbag play --clock <rrc_bag>.bag
```