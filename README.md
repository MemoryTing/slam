## Meshroom
AliceVision's binaries must be in the path while running Meshroom.
### Installed AliceVision
required :
1. CMake
2. Git
3. gcc
4. Boost
5. OpenEXR
6. OpenImageIO
7. zlib
8. OpenCV
---
can't found : 
1. MOSEK header , MOSEK library (好像是PATH沒有設定好？)
2. Alembic
3. UncertaintyTE headers , UncertaintyTE library
4. Geogram
5. OpenGV headers
---
不確定是不是有安裝成功或是找不到要怎麼裝 :
1. PopSift (feature extraction on GPU)
2. OpenMP (enable multi-threading)
3. CCTag (feature extraction/matching and localization on CPU or GPU)
4. Magma (required for UncertaintyTE)
5. Cuda >= 7.0 (feature extraction and depth map computation)
----
Download the Meshroom-2019.1.0-linux.tar.gz
upzip then click the Meshroom icon
nothing happened
use terminal to run it
Traceback (most recent call last):
  File "/opt/rh/rh-python36/root/usr/lib64/python3.6/site-packages/cx_Freeze/initscripts/__startup__.py", line 13, in run
  File "<frozen importlib._bootstrap>", line 971, in _find_and_load
  File "<frozen importlib._bootstrap>", line 955, in _find_and_load_unlocked
  File "<frozen importlib._bootstrap>", line 656, in _load_unlocked
  File "<frozen importlib._bootstrap>", line 626, in _load_backward_compatible
  File "/opt/Meshroom/setupInitScriptUnix.py", line 27, in <module>
OSError: [Errno 7] Argument list too long



## Blackbird
1. the drone 以及每台camera的位置![](http://volibear.cs.nthu.edu.tw:3000/uploads/upload_ff137ef8a84fc05c7e197a74c4114ea6.JPG)
2. 整個dataset的架構![](http://volibear.cs.nthu.edu.tw:3000/uploads/upload_ddbc556667afb70451795a61a9ffe748.JPG)
3. all files in BlackbirdDataset
https://github.com/mit-fast/Blackbird-Dataset
4. other files in BlackbirdDatasetData
http://blackbird-dataset.mit.edu/BlackbirdDatasetData/
5. video of yawConstant
http://blackbird-dataset.mit.edu/BlackbirdDatasetData/sphinx/yawConstant/maxSpeed3p0/videos/Ancient_Egypt_Museum_Room.mp4
6. video of yawForward
http://blackbird-dataset.mit.edu/BlackbirdDatasetData/sphinx/yawForward/maxSpeed3p0/videos/Ancient_Egypt_Museum_Room.mp4
7. 
![](http://volibear.cs.nthu.edu.tw:3000/uploads/upload_3759468b40a26dd956f40fa21ef3b158.JPG)
![](http://volibear.cs.nthu.edu.tw:3000/uploads/upload_5d18ad8685e44bbca5850af9edfb6b6f.JPG)
![](http://volibear.cs.nthu.edu.tw:3000/uploads/upload_94a198bf8995a7e72e9ab671ebe56350.JPG)

### projects
1. https://github.com/clydemcqueen/flock2
    - Latest commit on 27 Mar 2019
    - Ubuntu 18.04 ffmpeg 3.4.4 OpenCV 3.2
    - Python 3.6+ numpy 1.15.2 transformations 2018.9.5
    - flying one or more Tello drones
    - language : python
2. https://github.com/stytim/Drone_Visual_SLAM
    - Latest commit on 29 June 2018
    - using LSD-SLAM to robustly track the position of an AR drone
    - language : C++
3. https://github.com/raulmur/ORB_SLAM2?fbclid=IwAR2uYO-8Z58B2VPe9rNuGOdvswCJzaFClLRGBlRGuMyTROfVipkr-WiVfFs
    - Latest commit on 11 Oct 2017
    - tested in Ubuntu 12.04, 14.04 and 16.04
    - support OpenCV 3 and Eigen 3.3
    - for Monocular, Stereo and RGB-D cameras
    - language : C++
4. https://github.com/phooning/DroneRapid3DReconstruction
    - Latest commit on 21 April 2019
    - Allow drones to go from one point to another by itself without collision.
    - used Raspberry Pi ,OpenCV2 ,SDL2 ,NumPy ,SciKit
    - there is a demo video in folder footage
    - language : python

### not really sure what it is
1. https://github.com/Zarkopafilis/dronepilot
    - drone pilot
    - language : python
    - Latest commit on 14 Dec 2018
2. https://github.com/Ali-Hirani/uav-slam
    - Autonomous in-door drone navigation using a sensor based approach for SLAM
    - language : python
    - Latest commit on 16 Mar 2019
3. https://github.com/LKeaning/SLAM-Tutorial
    - implementaion of visual inertial SLAM with AR Drone
    - language : C++
    - Latest commit on 21 Feb 2019
. https://github.com/FlorianWilk/SPDR_1
    - Latest commit on 23 Sep 2018
    - use Arduino Mega Servo-Board
    - use a 360° LIDAR (light/laser based range detection) and a wide angle camera.
    - language : C++

## datasets
### drone
1. http://academictorrents.com/details/eb542a231dbeb2125e4ec88ddd18841a867c2656
整理一下它是什麼東東看一下paper抓一些video或是sample出來
### RGBD image
1. https://cs.nyu.edu/~silberman/datasets/nyu_depth_v2.html?fbclid=IwAR1Rf7pJe8QgidEdCAr80NX7hk9ZnLhlWWtYGdhRY1iIk2CYXtbKKarwiWw
2. https://vision.in.tum.de/data/datasets/rgbd-dataset
### autonomous driving
1. https://daniilidis-group.github.io/mvsec/
2. https://sites.google.com/view/multispectral/home
3. http://www.cvlibs.net/datasets/kitti/index.php?fbclid=IwAR1mqhIsCq2lMvDhphHqz8WhUAO8SlPHkYgDwAMGBB8rZcSmKFOBlsLJqdM
## 
1. https://www.hs-karlsruhe.de/odometry-data/
    - use plenoptic camera and a pair of stereo cameras
2. http://www.cvlibs.net/datasets/kitti/raw_data.php?type=residential
3. https://github.com/torrvision/CollaborativeSLAMDataset
    - use an Asus ZenFone AR augmented reality smartphone
4. https://interiornet.org/
5. https://vision.in.tum.de/data/datasets/intrinsic3d
    - Shape-from-Shading
    - spatially-varying spherical harmonics
    - highly to consistent surface texture recovery
