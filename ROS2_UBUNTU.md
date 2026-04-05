ROS2-COMMANDS-UBUNTU

UBUTNU

| Comando     | Descripción |
| ----------- | ------------ |
| Contenido 1 | Contenido 2  |
| Contenido 4 | Contenido 5  |
| Contenido 7 | Contenido 8  |

ROS2 - BEFORE START TO WORK 

| Comando                       | Descripción                      |
| ----------------------------- | --------------------------------- |
| ``cd /workspace``             | Enter in the  workspace ros2      |
| ``colcon build``              | Enter colcon build to charge data |
| ``source install/setup.bash`` | Enter the command to update data  |

ROS2 - CREATE PACKAGE

| Comando                                                                         | Descripción                                          |
| ------------------------------------------------------------------------------- | ----------------------------------------------------- |
| ``cd ~/workspace/src``                                                          | Enter in the folder src is in your workspace          |
| ``ros2 pkg create --build-type ament_python --node-name test_node name_folder`` | Create package                                        |
| ``UPDATE...``                                                                   | Update with colcon build in your folder cd /workspace |

ROS2 - GAZEBO

| Comando                                                   | Descripción                      |
| --------------------------------------------------------- | --------------------------------- |
| ``ros2 launch puzzlebot_gazebo gazebo_example_launch.py`` | Run the Puzzlebot gazebo simulato |

ROS2 - RUN PACKAGE AND NODE

| Comando                                                          | Descripción                                                                            |
| ---------------------------------------------------------------- | --------------------------------------------------------------------------------------- |
| ``ros2 run my_package my_node --ros-args -p use_sim_time:=True`` | Command line directly to make your node use the simulated time instead of the real time |

ROS2 - RUN LAUNCH

| Comando                                        | Descripción     |
| ---------------------------------------------- | ---------------- |
| ``ros2 launch mobile_robotics move.launch.py`` | Execute the node |

ROS2 - PUBLIC DATA  

| Comando                                                                | Descripción       |
| ---------------------------------------------------------------------- | ------------------ |
| ``ros2 topic pub --once /topic_name std_msgs/msg/Float32 "data: 1.0"`` | Send data by topic |

ROS2 - RVIZ2

| Comando                  | Descripción       |
| ------------------------ | ------------------ |
| ``ros2 run rviz2 rviz2`` | Run the simulation |

ROS2 - TF2 - Static

| Comando                                                                                       | Descripción        |
| --------------------------------------------------------------------------------------------- | ------------------- |
| ``ros2 run tf2_ros static_transform_publisher X Y Z roll pitch yaw name_referent_mark label`` | Publish static mark |

ROS2 - TF2 - Dynamic

| Comando | Descripción        |
| ------- | ------------------- |
|         | Publish static mark |

ROS2 - TF2 - install rqt-tf-tree

| Comando                                     | Descripción |
| ------------------------------------------- | ------------ |
| ``sudo apt install ros-humble-rqt-tf-tree`` | Download     |
| ``ros2 run rqt_tf_tree rqt_tf_tree``        | Running      |
| ``ros2 run tf2_ros tf2_echo robot1 world``  | Information  |

ROS2 - build packeges 

| Comando                                                                                                                                                         | Descripción   |
| --------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------- |
| ``ros2 pkg create --build-type ament_python puzzlebot_sim --dependencies std_msgs sensor_msgs geometry_msgs launch_ros tf2_ros rclpy robot_state_publisher joint_state_publisher_gui`` | Build packeges |

ROS2 - TF2 - install rqt-tf-tree

| Comando                                     | Descripción |
| ------------------------------------------- | ------------ |
| ``sudo apt install ros-humble-rqt-tf-tree`` | Download     |
| ``ros2 run rqt_tf_tree rqt_tf_tree``        | Running      |
| ``ros2 run tf2_ros tf2_echo robot1 world``  | Information  |

ROS2 - build packeges 

| Comando                                                                                                                                                         | Descripción                             |
| --------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------- |
| ``ros2 pkg create --build-type ament_python tf_examples --node-name static_tf --dependencies geometry_msgs python3-numpy rclpy tf2_ros_py ros2launch std_msgs`` | Build packeges in the folder /src        |
| chmod +x tf_examples/tf_examples/*                                                                                                                              | Give permitions of execution all scripts |
