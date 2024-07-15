# task1AI-WEEK3-
### ^^ Controlling the robot arm by (joint_state_publisher) and (Moveit and kinematics) <br> <br>
~~~
before we start, we make sure to ....
~~~

### Prepare our workspace  (i already did in my previous task) <br>

<img src=https://github.com/user-attachments/assets/ac41d888-c29d-4ac6-9c62-ef4da41cfda5 width=50%>

### - Install the Packages into our /catkin_ws/src
~~~
$ cd ~/catkin_ws/src
$ sudo apt install git
$ git clone https://github.com/smart-methods/arduino_robot_arm
~~~
### - Install all the dependencies 
~~~
$ cd ~/catkin_ws
$ rosdep install --from-paths src --ignore-src -r -y
$ sudo apt-get install ros-noetic-moveit
$ sudo apt-get install ros-noetic-joint-state-publisher ros-noetic-joint-state-publisher-gui
$ sudo apt-get install ros-noetic-gazebo-ros-control joint-state-publisher
$ sudo apt-get install ros-noetic-ros-controllers ros-noetic-ros-control
~~~
### - Compile the package
~~~
$ catkin_make
~~~

## ^ Controlling the robot arm by joint_state_publisher
---
~~~
$ source catkin_ws/devel/setup.bash
$ roslaunch robot_arm_pkg check_motors.launch
~~~

<img src=https://github.com/user-attachments/assets/1feab4f0-8e8b-4c99-b786-be396db872ec width=50%> <br>

~~~
$ roslaunch robot_arm_pkg check_motors_gazebo.launch
~~~

<img src=https://github.com/user-attachments/assets/d36998e9-7319-4cc5-91b6-e77f331ebba0 width=50%>


## ^ Controlling the robot arm by Moveit and kinematics
---
~~~
$ roslaunch moveit_pkg demo.launch
~~~
<img src=https://github.com/user-attachments/assets/e4ddfaee-9cd6-452a-806b-3dd082a07f14 width=50%>
