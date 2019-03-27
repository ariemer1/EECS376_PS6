#Controlling the arms on the Baxter Robot. these commands will tuck baxters arms

roslaunch worlds glennan_world.launch 
rosrun baxter_tools enable_robot.py -e 
rosrun baxter_tools tuck_arms.py -u 

#to control the arms from the command line use: 

rostopic pub /robot/right_joint_position_controller/joints/right_s0_controller/command std_msgs/Float64 VALUE
# EECS376_PS6
