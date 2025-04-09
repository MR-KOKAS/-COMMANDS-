
ROS2-COMMANDS-UBUNTU 

UBUTNU
| Comando         | Descripción     | 
|-----------------|-----------------|
| Contenido 1     | Contenido 2     | 
| Contenido 4     | Contenido 5     | 
| Contenido 7     | Contenido 8     | 


ROS2 - BEFORE START TO WORK 
| Comando         | Descripción     | 
|-----------------|-----------------|
| ```cd /workspace```    | Enter in the  workspace ros2    | 
| ```colcon build```    | Enter colcon build to charge data   | 
| ```source install/setup.bash```     | Enter the command to update data    | 

ROS2 - CREATE PACKAGE
| Comando         | Descripción     | 
|-----------------|-----------------|
|  ```cd ~/workspace/src```    | Enter in the folder src is in your workspace  | 
| ```ros2 pkg create --build-type ament_python --node-name test_node name_folder```    | Create package | 
| ```UPDATE...```    | Update with colcon build in your folder cd /workspace | 


ROS2 - GAZEBO
| Comando         | Descripción     | 
|-----------------|-----------------|
| ```ros2 launch puzzlebot_gazebo gazebo_example_launch.py```    | Run the Puzzlebot gazebo simulato  | 


ROS2 - RUN PACKAGE AND NODE
| Comando         | Descripción     | 
|-----------------|-----------------|
| ```ros2 run my_package my_node --ros-args -p use_sim_time:=True```    | Command line directly to make your node use the simulated time instead of the real time  | 

