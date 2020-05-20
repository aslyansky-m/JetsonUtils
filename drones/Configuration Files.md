# Configuration Files

## Calibration

Tried [Kalibr](https://github.com/ethz-asl/kalibr):

- [CDE](https://github.com/ethz-asl/kalibr/wiki/downloads) gives strange error
- failed to compile because of a bug
- need to fix

## Realsense D435i

- Intel's [whitepaper](https://www.intel.com/content/dam/support/us/en/documents/emerging-technologies/intel-realsense-technology/RealSense_Depth_D435i_IMU_Calib.pdf?language=en_US) on IMU calibration
- [emitter_disabled_60fps.json](https://github.com/engcang/rovio-application/blob/master/d435i/emitter_disabled_60fps.json) - need to find out how to configure the camera (e.g. disable the emitter programmatically)

## VINS

Found different configurations:

- [Official VINS](https://github.com/mhc994/VINS-Fusion/tree/wz_fly/config/realsense_d435i)
- [WilliamC17](https://www.cnblogs.com/williamc17/p/10748946.html)
- [vins-application/d435i](https://github.com/engcang/vins-application) - very informative
- also tried using results of online calibration

Notes:

- Decreasing accelerometer noise will lead to instability

## ROVIO

- [rovio-application/d435i](https://github.com/engcang/rovio-application/tree/master/d435i)
- [AerialRobotics-IITK](https://github.com/AerialRobotics-IITK/rovio/blob/master/cfg/rovio.info#L21)



