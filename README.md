# TurtleBot3 Installation
This tutorial for install Turtlebot3 package and Gazebo simulation.
# ROS Version
* Noetic
# Installing Dependent Packages
Open yor cmd and write the following  commands
* `cd ~/catkin_ws/src/`
* `git clone https://github.com/ROBOTIS-GIT/turtlebot3_msgs.git`
* `git clone https://github.com/ROBOTIS-GIT/turtlebot3.git`
* `cd ~/catkin_ws && catkin_make`

 There are three models of TurtleBot3 Burger, Waffle and WaffelPi.
 
![TurtleBotModels](https://user-images.githubusercontent.com/50454895/87253120-42dfa600-c481-11ea-899d-325cdfbff197.jpeg)

 To add your model write the following command to open the bashrc file 
 * `gedit ~/.bashrc`
 scrole down to bottom of the file and write the follwing line as you see in the image, then save and close the file
 * `export TURTLEBOT3_MODEL=burger`
    ![bashrcFile](https://user-images.githubusercontent.com/50454895/87253114-3bb89800-c481-11ea-8784-699f27eb388d.png)
 reload the bashrc file by this command
 * `source ~/.bashrc`
 # TurtuleBot3 simulation installing
 * `cd ~/catkin_ws/src/`
 * `git clone https://github.com/ROBOTIS-GIT/turtlebot3_simulations.git`
 * `cd ~/catkin_ws && catkin_make`
 to start simulation Turtlebote3 in an empty enviroment write this command
 * `roslaunch turtlebot3_gazebo turtlebot3_empty_world.launch`
 if you face the follwing problem in image, navigate the directory to devel file `cd ~ /catkin_ws/devel`  and write the following command
 * `source setup.bash` and rewrite the previous command to start simulation
  	
![launch](https://user-images.githubusercontent.com/50454895/87253119-407d4c00-c481-11ea-8b60-7071e4987609.png)
 
 
# The Result
* after you followed the previous steps the Gazebo simulatore will open as the image 
    
![gazeboWidow](https://user-images.githubusercontent.com/50454895/87253118-3fe4b580-c481-11ea-9180-f1288b752442.png)
        
        
* If you want this environment using to test SLAM write this command in new window
	* `roslaunch turtlebot3_gazebo turtlebot3_world.launch`
* If you face the previous problem follow the same step. 
* This window will open 
    
![gazeboanatherWindoe](https://user-images.githubusercontent.com/50454895/87253116-3eb38880-c481-11ea-8182-476055e79c6c.png)
  
  * If you want to move the TurtleBot with your keyboard, use this command in new window
  	* `roslaunch turtlebot3_teleop turtlebot3_teleop_key.launch`
	
![directions](https://user-images.githubusercontent.com/50454895/87253115-3e1af200-c481-11ea-9901-b2a4058354c6.png)
