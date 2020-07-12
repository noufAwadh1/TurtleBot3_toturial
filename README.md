# TurtleBot3 Installation
this tutorial for install Turtlebot package and Gazebo simulation.
# Installing Dependent Packages
Open yor cmd and write the following  commands
* `cd ~/catkin_ws/src/`
* `git clone https://github.com/ROBOTIS-GIT/turtlebot3_msgs.git`
* `git clone https://github.com/ROBOTIS-GIT/turtlebot3.git`
* `cd ~/catkin_ws && catkin_make`
 there are three models of TurtleBot3 Burger, Waffle and WaffelPi. to add your model write the following command to open the bashrc file 
 * `gedit ~/.bashrc`
 scrole down to bottom of the file and write the follwing line as you see in the image, then save and close the file
 * `export TURTLEBOT3_MODEL=burger`
   //////
 reload the bashrc file by this command
 * `source ~/.bashrc`
 # TurtuleBot simulation installing
 * `cd ~/catkin_ws/src/`
 * `git clone https://github.com/ROBOTIS-GIT/turtlebot3_simulations.git`
 * `cd ~/catkin_ws && catkin_make`
 to start simulation Turtlebote3 in an empty enviroment write this command
 * `roslaunch turtlebot3_gazebo turtlebot3_empty_world.launch`
 if you face the follwing problem in image navigate the directory to devel file `cd ~ /catkin_ws/devel`  and write the following command
 * `source setup.bash` and rewrite the previous command to start simulation
  	/////
 
 
# The Result
* after you followed the previous steps the Gazebo simulatore will open as the image 
       ///
        
        
* If you want this environment using to test SLAM write this command in new window
	* `roslaunch turtlebot3_gazebo turtlebot3_world.launch`
* If you face the previous problem follow the same step. This window will open 
 /////
  
  * If you want to move the TurtleBot with your keyboard, use this command in new window
  	* `roslaunch turtlebot3_teleop turtlebot3_teleop_key.launch`
