# ros-

I will explain to you how you can download & run it
- VirtualBox 
- Ubuntu 
- Ros

To download
VirtualBox = https://www.virtualbox.org/wiki/Downloads
ubuntu = https://releases.ubuntu.com/16.04/



1- Download VirtualBox and install it on the device



2- Download Ununtu and install it on the device



3 - open VirtualBox > machine > new

![image](https://user-images.githubusercontent.com/109594520/180608056-4bb32c55-935d-47a2-9eef-d5760e053088.png)

4 - Choose a name and then Next > Next > Next > Next

![11](https://user-images.githubusercontent.com/109594520/180608250-870d0795-734a-4525-b113-6d5ccde74abc.png)

5 - open the new fill > ROS_OSS 

![image](https://user-images.githubusercontent.com/109594520/180608437-f2e877d7-7431-4541-a0c3-f63ec393af14.png)

6 - Choose the movie in the place of ubuntu and install it correctly > Start 

![ww](https://user-images.githubusercontent.com/109594520/180608544-ba9a4080-b6b7-4d71-8cf8-c7a4eb276ec7.png)


7- Install Ubuntu > Continue > Continue > Continue > Continue

![ggg](https://user-images.githubusercontent.com/109594520/180608758-b1a76cbd-18ae-4929-ba94-c63a68a4f20c.png)

8 - Choose the username and password

9 - Search for terminal and select it 

![image](https://user-images.githubusercontent.com/109594520/180608981-ecbbcac4-69fa-4f2d-8a1e-eb56ec393d72.png)


10 - it will open 
11- And you just need to copy and paste the following commands to install ros , the website = https://s-m.com.sa/ros.txt 


sudo sh -c 'echo "deb http://packages.ros.org/ros/ubuntu $(lsb_release -sc) main" > /etc/apt/sources.list.d/ros-latest.list'

sudo apt-key adv --keyserver 'hkp://keyserver.ubuntu.com:80' --recv-key C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654

sudo apt-get update

sudo apt-get install ros-kinetic-desktop-full

apt-cache search ros-kinetic

echo "source /opt/ros/kinetic/setup.bash" >> ~/.bashrc
source ~/.bashrc

sudo apt install python-rosdep python-rosinstall python-rosinstall-generator python-wstool build-essential

sudo apt install python-rosdep

sudo rosdep init

rosdep update

sudo apt-get install ros-noetic-catkin

mkdir -p ~/catkin_ws/src

cd ~/catkin_ws/

catkin_make

cd ~/catkin_ws/src

git clone https://github.com/smart-methods/arduino_robot_arm.git 

cd ~/catkin_ws

rosdep install --from-paths src --ignore-src -r -y

sudo apt-get install ros-kinetic-moveit

sudo apt-get install ros-kinetic-joint-state-publisher ros-kinetic-joint-state-publisher-gui

sudo apt-get install ros-kinetic-gazebo-ros-control joint-state-publisher

sudo apt-get install ros-kinetic-ros-controllers ros-kinetic-ros-control

sudo nano ~/.bashrc

at the end of the (bashrc) file add the follwing line
(source /home/Hattan/catkin_ws/devel/setup.bash)    - // note = its so so so Important  
then 
ctrl + o

source ~/.bashrc

roslaunch robot_arm_pkg check_motors.launch



and in this code ros will open finaly 

![Screenshot 2022-07-22 185021](https://user-images.githubusercontent.com/109594520/180609224-c7f2c6e0-f75f-493f-98cb-1d5e82b7c292.png)


![Screenshot 2022-07-22 185343](https://user-images.githubusercontent.com/109594520/180609228-456a7d11-09ac-4215-9bf4-ee5b6b491490.png)



