# Arduino_Robot_Arm
First Task of Smart Methods training

Steps of Tasks :

First:

I used the codes in smart methods github account 

$ cd ~/catkin_ws/src

$ sudo apt install git

$ git clone https://github.com/smart-methods/arduino_robot_arm 


Second:

I creating a workspace for catkin by using this codes

$ mkdir -p ~/catkin_ws/src

$ cd ~/catkin_ws/

$ catkin_make

![1](https://user-images.githubusercontent.com/86194970/124404126-36afc100-dd42-11eb-8d7d-c8d8e1ea701f.jpg)

Then I make sure that these functions exist or install them again using the following codes:

$ cd ~/catkin_ws

$ rosdep install --from-paths src --ignore-src -r -y

$ sudo apt-get install ros-melodic-moveit

$ sudo apt-get install ros-melodic-joint-state-publisher ros-melodic-joint-state-publisher-gui

$ sudo apt-get install ros-melodic-gazebo-ros-control joint-state-publisher

$ sudo apt-get install ros-melodic-ros-controllers ros-melodic-ros-control

Third: 

I can lunch the backage by using this codes:

$ roslaunch robot_arm_pkg check_motors.launch

![WhatsApp Image 2021-07-05 at 3 19 20 AM](https://user-images.githubusercontent.com/86194970/124404275-f43ab400-dd42-11eb-8f01-9e82d2b5188d.jpeg)

$ roslaunch robot_arm_pkg check_motors_gazebo.launch

![WhatsApp Image 2021-07-05 at 3 23 55 AM (1)](https://user-images.githubusercontent.com/86194970/124404294-087eb100-dd43-11eb-9737-c2f71476de07.jpeg)

$ roslaunch moveit_pkg demo.launch

![WhatsApp Image 2021-07-05 at 3 23 55 AM](https://user-images.githubusercontent.com/86194970/124404340-2f3ce780-dd43-11eb-96bd-51709715b5f9.jpeg)
