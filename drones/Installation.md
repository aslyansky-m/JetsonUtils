# Installation

## Jetpack

1. go to [nvidia](https://developer.nvidia.com/embedded/jetpack), install the SDK

2. choose target hardware, select all the packages

3. reboot Jetson in recovery mode: follow the guide, use```lsusb``` for debug

4. had this [issue](https://devtalk.nvidia.com/default/topic/1048803/jetson-tx2/sdk-manager-could-not-detect-target-hardware/4), solved by 
   ```sudo apt purge tlp tlp-rdw``` 

5. flash OS image, then configure the system, then proceed to installing all the packages

## ROS

#### Jetpack 3.3

1. Go to [installROSTX2](https://github.com/jetsonhacks/installROSTX2) repo, clone and run 

   ```.\installROS.sh -p ros-kinetic-desktop-full ```

2. Setup **catkin_ws** environment

#### Jetpack 4.2(3)

See [Jeson Zoo](https://elinux.org/Jetson_Zoo)\ROS:

```
# enable all Ubuntu packages:
sudo apt-add-repository universe
sudo apt-add-repository multiverse
sudo apt-add-repository restricted

# add ROS repository to apt sources
sudo sh -c 'echo "deb http://packages.ros.org/ros/ubuntu $(lsb_release -sc) main" > /etc/apt/sources.list.d/ros-latest.list'
sudo apt-key adv --keyserver 'hkp://keyserver.ubuntu.com:80' --recv-key C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654

# install ROS Base
sudo apt-get update
sudo apt-get install ros-melodic-ros-base

# add ROS paths to environment
sudo sh -c 'echo "source /opt/ros/melodic/setup.bash" >> ~/.bashrc'
```

## RealSense

1. Follow the [instructions](https://github.com/IntelRealSense/librealsense/blob/master/doc/installation_jetson.md) to install the SDK

2. Install [ddynamic_reconfigure](https://github.com/pal-robotics/ddynamic_reconfigure)

3. Install **cv_bridge**:

   ```git clone --single-branch --branch opencv4 https://github.com/fizyr-forks/vision_opencv.git```

4. Install [realsense-ros](https://github.com/IntelRealSense/realsense-ros) 

## Deep Learning

See [Jeson Zoo](https://elinux.org/Jetson_Zoo)







