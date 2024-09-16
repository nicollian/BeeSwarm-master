catkin_make -DPYTHON_EXECUTABLE=/usr/bin/python3

source devel/setup.bash

roslaunch bee_quadrotor gazebo.launch

roslaunch swarm_control start.launch

cd  ~/BeeSwarm/BeeSwarm/src/bee_quadrotor/script

python r9_single.py