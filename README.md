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
 
 13. xoa chạy lại trước catkin make , làm sạch hoàn toàn, xóa cả thư mục
 rm -rf ~/catkin_ws/build
 echo "source ~/catkin_ws/devel/setup.bash" >> ~/.bashrc
source ~/.bashrc

 14.
rosrun map_server map_saver -f ~/catkin_ws/src/baocao/src/maps/my_map
  chạy và lưu bản đồ 
eog ~/catkin_ws/src/baocao/src/maps/my_map.pgm
  bằng trình xem ảnh
 cat ~/catkin_ws/src/baocao/src/maps/my_map.yaml
   File này sẽ chứa thông tin như độ phân giải, gốc bản đồ, v.v.

 16.
 
 17. source devel/setup.bash

 18. reset môi trường của gazebo
     killall gzserver gzclient roslaunch
rm -rf ~/.gazebo/*
rm -rf ~/.ros/log/*


rostopic echo /scanroslaunch urdf_tutorial display.launch model:=$HOME/k67_ws/src/urdf/my_car.urdf
](https://git-scm.com/downloads)

rostopic echo /joint_states


https://drive.google.com/drive/folders/1aydmQNC4h1NfkZR4bfXoRGj94G5g9x_J?usp=drive_link
