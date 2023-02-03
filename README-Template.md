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
```
roslaunch raspimouse_gazebo main_20robots.launch
```

### Installing

* How/where to download your program
* Any modifications needed to be made to files/folders

### Executing program

* How to run the program
* Step-by-step bullets
```
code blocks for commands
```

## Help

Any advise for common problems or issues.
```
command to run if program contains helper info
```

## Authors

Contributors names and contact info

ex. Dominique Pizzie  
ex. [@DomPizzie](https://twitter.com/dompizzie)

## Version History

* 0.2
    * Various bug fixes and optimizations
    * See [commit change]() or See [release history]()
* 0.1
    * Initial Release

## License

This project is licensed under the [NAME HERE] License - see the LICENSE.md file for details

## Acknowledgments

Inspiration, code snippets, etc.
* [awesome-readme](https://github.com/matiassingers/awesome-readme)
* [PurpleBooth](https://gist.github.com/PurpleBooth/109311bb0361f32d87a2)
* [dbader](https://github.com/dbader/readme-template)
* [zenorocha](https://gist.github.com/zenorocha/4526327)
* [fvcproductions](https://gist.github.com/fvcproductions/1bfc2d4aecb01a834b46)
