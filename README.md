# chess_baxter
 A simulation of Baxter playing Chess using ROS system in Gazebo and Rviz.

 
Run the following commands on terminals:

Terminal 1:
``bash
roslaunch baxter_gazebo baxter_world.launch
``

Terminal 2:
``bash
rosrun baxter_tools enable_robot.py -e /n
rosrun baxter_interface joint_trajectory_action_server.py
``

Terminal 3:
``bash
roslaunch baxter_moveit_config baxter_grippers.launch
``

Terminal 4:
``bash
rosrun chess_baxter spawn_chessboard.py
``

Terminal 5:
``bash
rosrun chess_baxter pick_and_plave_moveit.py
``

Terminal 6:
``bash
rosrun chess_baxter gazebo2tfframe.py
``

At last, to delete the game, run:
``bash
rosrun chess_baxter delete_chessgame.py
``

Demo: https://youtu.be/SP-X_PM4qQM
