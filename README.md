# icart_ros2_sim
orneシリーズのシミュレータ(ros2)試作版
![image](https://github.com/haruyama8940/icart_ros2_sim/assets/68257043/ebb90fc0-afbb-4992-b669-690f845113c8)


# Install
依存パッケージのインストール
```
sudo apt install ros-foxy-gazebo-ros
sudo apt install ros-foxy-xacro
sudo apt install ros-foxy-joint-state-publisher-gui
sudo apt install ros-foxy-robot-state-publisher
```
```
git clone https://github.com/haruyama8940/icart_ros2_sim.git
git clone https://bitbucket.org/DataspeedInc/velodyne_simulator.git -b foxy-devel
```
# Build
```
cd ~/catkin_ws
colcon build --symlink-install
source ~/catkin_ws/install/setup.bash
```

#Launch
urdfを表示
```
ros2 launch icart_description display.launch.py 
```
シミュレータ(gazebo)を起動
```
ros2 launch icart_simulation box_cit3f.launch.py
```
