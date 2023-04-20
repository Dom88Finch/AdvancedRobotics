
# Robotic Arm Project
Code developed by Dominic Nzimi, QMUL

![ROS](http://wiki.ros.org/) is a Robotic Framework used for devoloping Robots. The video below shows how you can use ROS framework to with RViz to control a Robotic Arm. To achieve this, we first need to code up the plan for the robotic arm movement. This enables us to control the different joints of the arm and ensure the trajectory planning is stable.

<video src="https://user-images.githubusercontent.com/57221218/230620302-cb8a3fbf-b0f5-4b47-8143-cacc5786eb4f.mp4"></video>

The following system is run on ```Ubuntu``` and requires installation of ```ROS``` distribution onto computer.

To Run the package, open a terminal and run the follwiong comands after you have installed ```ROS```:

The command below downloads the required packages and ```![ROS melodic](http://wiki.ros.org/melodic)``` onto your linux device. (If you do not have a Linux machine, you can run the code on a virtual machine: a few links are provided below:
- Windows: https://www.virtualbox.org/
- MAC: https://mac.getutm.app/
)
```git clone -b melodic-devel https://github.com/ros-planning/panda_moveit_config.git rosdep updaterosdep install --from-paths . --ignore-src -r -y```

where ROS- DISTRO is the name of your ROS distribution.

  1. unzip the ```ar_week10_test.zip``` folder in the src folder.

  2. build the catkin workspace using (```catkin_make```)

  3. run the following on __four__ different terminals and ensure you source at each terminal using “ ```source devel/setup.bash```

    - ```roslaunch panda_moveit_config demo.launch```
    - ```rosrun ar_week10_test square_size_generator.py```
    - ```rosrun ar_week10_test move_panda_square.py```
    - ```rosrun rqt_plot rqt_plot```



