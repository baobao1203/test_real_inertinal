 1. create folder
mkdir -p ~/ros_ws/src

 2. move on folder 
cd ~/ros_ws

 3. make agan catkin_make
 source devel/setup.bash
 
 4. create do work  
 catkin_create_pkg my_robot std_msgs roscpp rospy

 6. control robot by keybach
 rostopic echo /cmd_vel
 rosrun teleop_twist_keyboard teleop_twist_keyboard.py _speed:=2.0 _turn:=3.0
 
 7. use rviz  
roslaunch urdf_tutorial display.launch model:=$HOME/NCKH/src/my_robot/baocao\(1\).urdf
 
 8. check file urdf 
 check_urdf /home/bao/k67_ws/src/mo_phong_robot/base.urdf

 9. cấp quyền đọc file 
 chmod +r /home/bao/catkin_ws/src/baocao/meshes/base.stl
 10.
 
 11. use launch 
 roslaunch baocao bao1.launch 
 
 12.bé hơn launch 
 rosrun gazebo_ros spawn_model -file ~/k67_ws/src/bao/urdf/xe_bus.urdf -urdf -model bus_1
 
 13. xoa chạy lại trước catkin make 
 rm -rf ~/catkin_ws/build

 14.
 

 15.
 
 16. source devel/setup.bash


rostopic echo /scanroslaunch urdf_tutorial display.launch model:=$HOME/k67_ws/src/urdf/my_car.urdf
](https://git-scm.com/downloads)

rostopic echo /joint_states


