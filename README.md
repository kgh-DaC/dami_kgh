mkdir ~/catkin_ws

mkdir ~/catkin_ws/src

cd ~/catkin_ws/src

git clone https://github.com/kgh-DaC/dami_kgh.git

cd ~
git clone https://github.com/introlab/rtabmap.git rtabmap
cd rtabmap/build
cmake ..
make -j1
sudo make install


cd ~/catkin_ws
sudo apt update
sudo apt upgrade

sudo apt-get install ros-noetic-geographic-*

sudo apt-get install geographiclib-*

sudo apt-get install libgeographic-*

sudo apt-get install ros-noetic-rtabmap-ros 

catkin_make -j1
