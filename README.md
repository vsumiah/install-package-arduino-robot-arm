# install-package-arduino-robot-arm
# To stabilise the arm's package, we will use a number of steps that will help us smoothly!

1.Go to the basic orders of https://s-m.com.sa/ros.txt

2.Start copying and fasten orders in Ubuntu terminal from line 13

3.Since my version is noetic, we will follow the same orders.
~~~
$ Mkdir -p ~/catkin_ws/src

$ Cd ~/catkin_ws/

$ Catkin_make

$ Cd ~/catkin_ws/src

$ Git clone https://github.com/smart-methods/arduino_robot_arm.git

$ Cd ~/catkin_ws
~~~
~~~
$ rosdep install —from-paths src —ignore-src -r -y
~~~

~~~
$ Sudo apt-get install ros-noetic-moveit

$ Sudo apt-get install ros-noetic-joint-state-publisher ros-noetic-joint-state-publisher-gui

$ Sudo apt-get install ros-noetic-gazebo-ros-control joint-state-publisher

$ Sudo apt-get install ros-noetic-ros-controllers Ros-noetic-ros-control
~~~

~~~
$ Sudo nano ~/.bashrc
~~~

*At the end of the (bashrc) file add the follwing line
(Source /home/sumiah/catkin_ws/devel/setup.bash)
Then

Ctrl + o
~~~
$ ~/.bashrc source
~~~
4.And here we will come up with the last thing that will help us open the arm!
~~~
$roslaunch robot_arm_pkg check_motors.launch
~~~
![2022-07-26 (1)](https://user-images.githubusercontent.com/108010896/181042152-929bb2d3-091e-4bd3-a7ba-8296d2b82d31.png)

https://user-images.githubusercontent.com/108010896/181042246-950ae5ea-bf0a-4bcf-ba27-46a5baacef74.mp4

**In short, these steps, and when the footage appears above, it means that the package  has been successfully stabilised!**
