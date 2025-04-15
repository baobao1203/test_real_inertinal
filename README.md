rostopic echo /scanroslaunch urdf_tutorial display.launch model:=$HOME/k67_ws/src/urdf/my_car.urdf
](https://git-scm.com/downloads)
rosrun teleop_twist_keyboard teleop_twist_keyboard.py _speed:=2.0 _turn:=3.0
rostopic echo /cmd_vel
rostopic echo /joint_states
