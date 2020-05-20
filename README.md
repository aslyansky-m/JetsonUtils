# JetsonUtils
Useful links for developing with Jetson

## IDE's and tools
#### VS Code

```
sudo apt-get install curl
curl -L https://github.com/toolboc/vscode/releases/download/1.32.3/code-oss_1.32.3-arm64.deb -o code-oss_1.32.3-arm64.deb  
sudo dpkg -i code-oss_1.32.3-arm64.deb
code-oss 
```
#### Pycharm

```
sudo apt-get install openjdk-8-jdk
sudo apt-get install qt5-default qtbase5-dev qt5-doc qtcreator
```
then go to:
[Pycharm page](https://www.jetbrains.com/pycharm/download/#section=linux)

#### CMake
How to install the latest version: [link](https://askubuntu.com/questions/1125808/how-to-upgrade-cmake-in-arm-based-ubuntu)

## Power and performance

#### Modes
MAXN - the strongest

#### GPU Monitor
See [jtop](https://github.com/rbonghi/jetson_stats/wiki/jtop):
```
sudo -H pip install -U jetson-stats
```

#### HW Encode/Decode
See [Accelerated Gstreamer User Guide.pdf](https://developer.download.nvidia.com/embedded/L4T/r32_Release_v1.0/Docs/Accelerated_GStreamer_User_Guide.pdf?Th_8yVlnzo_EscxSbhZf_Auu019J1CCSx0nTM6syWjq_t9T7wp2WrMqahWYwVZOWyMzJGjAjDQ8S7Zmrc_E88jQ_-07MoNvm3focJriqJ16tG2YYRb04XJLXGwQFH5CFYWo0zjyyWHK8XE17qhq_L4ojHaGPRSeBLHLNw0_pKM4B55J-96U)

## Packages 

#### Offline installation:
[link](https://askubuntu.com/questions/15211/saving-deb-files-from-repositories-to-a-custom-location-for-installing-offline):
`sudo apt-get --download-only install packagename`

#### OpenCV
See [here](https://jkjung-avt.github.io/opencv3-on-tx2/)
