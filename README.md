# ROBOTICS EVALUATION TOOLKITS
A simulation of basic robot localization (SLAM) and navigation in warehouse environment

**Author:** [Wang Han](http://wanghan.pro), Nanyang Technological University, Singapore


## 1. Evaluation
### 1.1. Simulation Description
This package provides a simulation environment of warehouse. A robot is simulated at the center of the environment, with 2D laser scanner provided. 
<p align='center'>
<img width="65%" src="/img/warehouse.gif"/>
</p>

### 1.2. robot tutorial
The localization and navigation unit is also provided for evaluation. This inlcudes basic 2D slam and robot navigation algorithm.
<p align='center'>
<img width="95%" src="/img/warehouse_simulation.gif"/>
</p>

### 1.3. 3D mapping
The robot model is equipped with 3D Lidar as an alternative and simulation of 3D mapping is available 
<p align='center'>
<img width="95%" src="/img/3d_mapping.gif"/>
</p>

## 2. Prerequisites
### 2.1 **Ubuntu** and **ROS**
Ubuntu 64-bit 18.04.

ROS Melodic. [ROS Installation](http://wiki.ros.org/ROS/Installation)

### 2.2. **ROS Package**
```
sudo apt-get install ros-melodic-hector-trajectory-server ros-melodic-slam-gmapping ros-melodic-navigation
```

## 3. Build 
### 3.1 Clone repository:
```
    cd ~/catkin_ws/src
    git clone https://github.com/wh200720041/warehouse_navigation.git
    cd ..
    catkin_make
    source ~/catkin_ws/devel/setup.bash
```

### 3.2 Launch ROS
```
    roslaunch warehouse_simulation warehouse_simulation.launch
```
Note that it takes a few minutes to load model upon first launch

### 3.3 Robot Control
You can use keyboard (arrow keys) to manually control the robot (select cmd window first)

### 3.4 Autonomous Navigation
You may set target points in RVIZ and the robot will navigate to the location in gazebo.
1. click 2d nav goal button on rviz
2. click any points you want on the map


## 4.Acknowledgements
Thanks for the great work from [GEAR](https://bitbucket.org/osrf/ariac/src/master/).


