Usage:
=================

1. download KITTI odometry ground truth datas to "PATH/TO/WORKSPACE/dataset/poses"
2. build target :
```
g++ -O3 -DNDEBUG -o evaluate_odometry evaluate_odometry.cpp matrix.cpp
```
3. put target <evaluaate_odometry> to your SLAM eval workspace.
4. usage:
```
./evaluate_odometry {PATH/TO/YOUR/SLAM/RESULT} {KITTI_SEQUENCE_NUMBER}

for example:
./evaluate_odometry ./CameraTrajectory.txt 2
```
