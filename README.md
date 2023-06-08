source install/setup.bash
ros2 launch drone_sim launch_sim.launch.py world:=/home/gleb/Documents/Programming/drone_sim_ws/src/drone_sim/worlds/basic.world

source install/setup.bash
ros2 run teleop_twist_keyboard teleop_twist_keyboard --ros-args -r /cmd_vel:=/diff_cont/cmd_vel_unstamped

rviz2