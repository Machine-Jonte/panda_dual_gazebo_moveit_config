# MoveIt! dual panda robots (Franka Emika)
## Introduction
This is a moveit configuration for controlling 2 Franka Emika robots in gazebo.

## Requierments
You need to download the package dual_panda_gazebo for using this package (where the xacro file is). [That package is available on my github](https://github.com/Machine-Jonte/panda_dual_gazebo_moveit_config).


# How to setup MoveIt!
How this package was build:
* Follow MoveIt! configuration setup
* Configure controllers (see moveit_controllers.yaml and ros_controllers.yaml)
* Write moveit_planning_execution.launch (meta file for launching everything) and panda_dual_control.launch (launch controllers). Uncommented line in gazebo.launch to avoid launching the controllers twice.
* DON'T RUN JOINT STATE PUBLISHER WHEN RUNNING GAZEBO. It will interfere.
