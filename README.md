
# ROBOTICS EVALUATION TOOLKITS
A simulation of basic robot localization (SLAM) and navigation in warehouse environment

**Author:** [Wang Han](http://wanghan.pro), Nanyang Technological University, Singapore


## 1. Evaluation
### 1.1. Simulation Description
This package provides a simulation environment of warehouse. A robot is simulated at the center of the environment, with 2D laser scanner provided. 
<p align='center'>
<img width="65%" src="/img/warehouse.gif"/>
</p>

### 1.2. Robot Simulation
<p align='center'>
<img width="95%" src="/img/warehouse_simulation.gif"/>
</p>


## 2. Prerequisites
### 2.1 **Ubuntu** and **ROS**
Ubuntu 64-bit 18.04.

ROS Melodic. [ROS Installation](http://wiki.ros.org/ROS/Installation)

### 2.2. **ROS Package**
```
sudo apt-get install ros-melodic-gazebo-ros
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


## 4.Acknowledgements
Thanks for the great work from [GEAR](https://bitbucket.org/osrf/ariac/src/master/).

