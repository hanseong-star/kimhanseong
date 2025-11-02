# Limo

## Build from source code


```bash
# 1) workspace 준비
mkdir -p ~/catkin_ws/src && cd ~/catkin_ws/src

# 2) package 생성
cd ~/limo_ws/src
catkin_create_pkg limo_lane roscpp rospy ...
#package name = limo_lane 뒤에는 필요한 package

\
ex) 카메라 package

```bash
catkin_create_pkg limo_lane roscpp rospy std_msgs sensor_msgs cv_bridge image_transport

# 3) 파일 넣기
#python이면 scripts
#c++ 이면 src

# 4) 실행 권한 python만
chmod +x ~/limo_ws/src/limo_lane/scripts/lane_node.py

# 5) 빌드
cd ~/limo_ws
catkin_make
source devel/setup.bash

# 6) 실행
roslaunch limo_lane lane_node.launch

