# Multiple RaspberryPiMouse robots simulator

Gazebo simulator for multiple RT RaspberryPiMouse robots
The same as https://github.com/keeratifts/Multiple-RaspberryPiMouse-robots-simulator#multiple-raspberrypimouse-robots-simulator
Only changes is the name change from 'Multiple-RaspberryPiMouse-robots-simulator' to 'robot_environment'

## Requirements

* Computer
   * ROS
      * [Kinetic Kame](http://wiki.ros.org/kinetic/Installation/Ubuntu)
      * [Melodic Morenia](http://wiki.ros.org/melodic/Installation/Ubuntu)
      * [Noetic Ninjemys](http://wiki.ros.org/noetic/Installation/Ubuntu)
   * Gazebo
      * Gazebo 9.x

## Installation

Download this package & install all system dependecies

```
cd ~/<your_workspace>/src
git clone https://github.com/keeratifts/Multiple-RaspberryPiMouse-robots-simulator.git
git clone https://github.com/ryuichiueda/raspimouse_ros_2.git
rosdep install raspimouse_ros_2
cd ~/<your_workspace>/src/Multiple-RaspberryPiMouse-robots-simulator
rosdep install -r -y -i --from-paths raspimouse*
```

Build up this package
```
cd ~/<your_workspace>
catkin_make
source devel/setup.bash
```

Download the Gazebo model
```
rosrun raspimouse_gazebo download_gazebo_models.sh
```

### Getting started

Enter the following command for single robot simulator.
![single_bots](https://user-images.githubusercontent.com/124341547/216545614-33680131-e06c-4087-9902-6f612e4bd28e.png)
```
roslaunch raspimouse_gazebo main_singlerobot.launch 
```

Enter the following command for 2 robots simulator.
![two_bots](https://user-images.githubusercontent.com/124341547/216545811-ba9b18c5-d6c0-4d5f-bea4-959831b4aad3.png)
```
roslaunch raspimouse_gazebo main_2robots.launch
```

Enter the following command for 20 robots simulator.
![twenty_bots](https://user-images.githubusercontent.com/124341547/216554855-e6a1203c-6cfe-4244-847d-77e4b3c45d4a.png)
```
roslaunch raspimouse_gazebo main_20robots.launch
```

Enter the following command for 8 multicolor-robots simulator in the crossroad scenario.
![trafficlights_bots](https://user-images.githubusercontent.com/124341547/216554913-5593dbe5-27f6-4f28-a74b-49c028adc7fc.png)
```
roslaunch raspimouse_gazebo main_multicolor.launch 
```
