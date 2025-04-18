mkdir -p ~/ros_ws/src
cd ~/ros_ws
catkin_make
source devel/setup.bash

catkin_create_pkg my_robot std_msgs roscpp rospy

rostopic echo /scanroslaunch urdf_tutorial display.launch model:=$HOME/k67_ws/src/urdf/my_car.urdf
](https://git-scm.com/downloads)
rosrun teleop_twist_keyboard teleop_twist_keyboard.py _speed:=2.0 _turn:=3.0
rostopic echo /cmd_vel
rostopic echo /joint_states
roslaunch urdf_tutorial display.launch model:=$HOME/NCKH/src/my_robot/baocao\(1\).urdf
check_urdf /home/bao/k67_ws/src/mo_phong_robot/base.urdf
