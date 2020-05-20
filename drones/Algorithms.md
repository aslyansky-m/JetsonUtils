## Algorithms

#### VINS-Fusion

- succeeds with good lighting
- struggles with some sequences at night
- needs tuning of feature tracking parameters for night
- struggles with high frequency shakes due to IMU instability
- future work focuses on better low-light tracking

#### ROVIO

- started testing
- in some cases kind of works

## Some Conclusions

- need light which has uniform illumination at plane (and not sphere)
- need better IMU
- when illumination is high exposure time shortens and you get flickers from PWM



## Illumination resilience 

- add photometric error to [PyrLK](https://github.com/opencv/opencv_contrib/blob/863d6ad3919473cf3cb9b850c3ce428b16faa9b0/modules/cudaoptflow/src/cuda/pyrlk.cu)
- [ IMU-aided Affine-photometric KLT](http://www.cs.cmu.edu/~myung/IMU_KLT/KLT_gpu_cuda.html)